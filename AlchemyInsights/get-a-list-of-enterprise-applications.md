---
title: 응용 프로그램 목록 Enterprise
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116734"
---
# <a name="get-a-list-of-enterprise-applications"></a>응용 프로그램 목록 Enterprise

1. Powershell 명령을 통해 엔터프라이즈 응용 프로그램(모든 응용 프로그램 또는 표시 이름, ID, 식별자 URIS 등으로 필터링)의 목록을 얻거나 [Get-AzureADApplication (AzureAD)을](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)참조하세요. 
2. Powershell 명령을 통해 서비스 사용자 개체(모든 개체 또는 ID로 필터링된 개체) 목록을 얻하려면 [Get-AzureADServicePrincipal (AzureAD)를](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)참조하세요.
3. SAML로 구성된 앱 목록을 얻게 하려는 경우 **PowerShell** 스크립트를 따라 다음 작업을 하는 것이 도움이 될 수 있습니다.

    모든 응용 프로그램이 OAuth 앱 또는 SAML 앱(갤러리 앱과 갤러리 앱이 아닌 앱 모두)이면 등록이 진행될 때 AAD에서 두 개의 개체가 만들어집니다. 하나는 Application 개체라고, 다른 하나는 Service Principal 개체입니다. PowerShell을 사용하여 서비스 사용자 개체의 속성을 덤프하면 모든 응용 프로그램에 특정 수의 태그가 연결되어 있는 것을 발견할 수 있습니다.

    - OAuth 앱에는 **"WindowsAzureActiveDirectoryIntegratedApp" 태그가 있습니다.**
    - 갤러리 SAML 앱에는 **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1"** 태그가 있습니다.
    - 갤러리가 아닌 SAML 앱에는 **"WindowsAzureActiveDirectoryCustomSingleSignOnApplication" 태그가 있습니다.**

    따라서 이러한 태그를 사용하여 앱의 종류를 찾을 수 있습니다. **"WindowsAzureActiveDirectoryIntegratedApp"** 태그는 모든 유형의 앱에서 일반적입니다. 다음 코드 코드 일부를 사용하여 모든 SAML 앱(갤러리와 갤러리가 아닌 앱 모두)을 나열할 수 있습니다.

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    자세한 내용은 [Azure AD에서 SAML 사용 앱 식별을 참조하세요.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **웹 응용 프로그램만** 찾아서 나열: 다음 명령을 사용하여 응용 프로그램 유형이 "Web app/API"인 모든 Azure AD 응용 프로그램을 다운로드합니다.

    Get-AzureADApplication -All:$true | Where-Object { $_를 사용합니다. PublicClient -ne $true } | FT
5. **네이티브 응용 프로그램만 찾아서** 나열: 다음 명령을 실행하여 모든 기본 클라이언트(데스크톱/모바일 장치) 응용 프로그램을 얻습니다.

    Get-AzureADApplication -All:$true | Where-Object { $_를 사용합니다. PublicClient -eq $true } | FT
6. 등록된 모든 Azure AD 응용 프로그램 세부 정보를 **CSV로** 내보내기: 아래 명령은 필요한 세부 정보가 있는 모든 Azure AD 앱을 csv 파일로 내보낼 수 있습니다.

    - Get-AzureADApplication -All:$true | Select-Object, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. 사용되지 않는 Azure 앱 목록을 **내보내야 합니다.** – 감사 보고서

    Azure AD는 라이선스가 있는 경우 최대 30일 동안만 응용 프로그램 로그를 Azure AD Premium 있습니다.
    데이터를 30일 이상 보존하는 두 가지 옵션이 있습니다. Azure AD [보고 API를](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) 사용하여 프로그래밍식으로 데이터를 검색하고 데이터베이스에 저장할 수 있습니다. 또는 감사 로그를 타사 SIEM 시스템에 통합할 수 있습니다.

    또한 모든 응용 프로그램 및 소유 응용 프로그램에 대한 앱 목록을 Azure Active Directory>앱 등록에서 모든 응용 프로그램/소유 응용>>다운로드할 수 있습니다.

    MS 응용 프로그램을 통해 응용 프로그램 목록을 Graph 응용 프로그램 목록 - Microsoft Graph [v1.0](https://docs.microsoft.com/graph/api/application-list) 및 응용 프로그램 리소스 유형 - Microsoft Graph [v1.0을 참조하세요.](https://docs.microsoft.com/graph/api/resources/application)
