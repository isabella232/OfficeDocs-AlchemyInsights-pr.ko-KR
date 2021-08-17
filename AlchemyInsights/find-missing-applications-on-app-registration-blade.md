---
title: 앱 등록 블레이드에서 누락된 응용 프로그램 찾기
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
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057108"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>앱 등록 블레이드에서 누락된 응용 프로그램 찾기

1. 앱 등록 포털에서 응용 프로그램을 찾을 수 없습니다.

    응용 프로그램이 다중 테넌트 응용 프로그램인 경우 다른 테넌트에 등록된 응용 프로그램은 앱 등록 블레이드 아래에 표시되지 않습니다. 그러나 테넌트에서 서비스 Enterprise 액세스한 후 서비스 사용자에 액세스한 후 Enterprise 응용 프로그램 블레이드에서 찾을 수 있습니다. 자세한 내용은 Azure AD의 & 앱 서비스 계정을 [참조하세요. - Microsoft ID 플랫폼.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. 관리자인 경우에도 앱 등록 블레이드에서 앱을 볼 수 없습니다.

    Azure Portal의 올바른 디렉터리에 있습니다.
3. 응용 프로그램이 Enterprise 응용 프로그램 블레이드 아래에는 나열되지 않지만 PowerShell 명령을 쿼리할 때 표시됩니다.

    경우에 따라 Azure Portal에서 응용 프로그램을 삭제한 후 포털에 응용 프로그램이 표시되지 않지만 완전히 삭제되지는 않을 수 있습니다. 자세한 내용은 다음 항목을 참조하세요.
    - Powershell 명령 **Get-AzureADDeletedApplication을** 사용하여 이전에 삭제한 응용 프로그램 목록을 검색하고 응용 프로그램이 목록에 표시될지 알 수 있습니다. 자세한 내용은 [Get-AzureADDeletedApplication (AzureAD)을 참조하세요.](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - 응용 프로그램을 완전히 제거하려면 PowerShell에서 다음을 시도해 볼 수 있습니다. **Remove-AzureADApplication -ObjectId**. 자세한 내용은 [Remove-AzureADApplication (AzureAD)을 참조하세요.](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - 또는 **AzureADDeletedApplication -ObjectId** 복원 Powershell 명령을 사용하여 삭제된 응용 프로그램을 복원할 수 있습니다. 자세한 내용은 [Restore-AzureADDeletedApplication (AzureAD)을 참조하세요.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. 새 Azure 테넌트에 미리 설치된 모든 엔터프라이즈 응용 프로그램의 목록을 찾을 수 없습니다.

    Azure AD에는 기본적으로 미리 설치된 엔터프라이즈 응용 프로그램이 없습니다. Azure AD 갤러리에서 찾아보거나 갤러리가 아닌 응용 프로그램을 추가하여 '새 응용 프로그램' 옵션에서 수동으로 추가해야 합니다. 자세한 내용은 [빠른 시작: Azure AD(Azure Active Directory 테넌트에 응용 프로그램 추가)를 참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    전역 관리자인 경우 앱 관리자 를 사용하여 앱에 [Microsoft 365 쉽게 액세스할 시작 관리자.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. 내 앱 포털에서 내 앱을 찾을 수 없습니다.

    앱이 내 앱 컬렉션 페이지에 숨겨져 있지 않은지 확인하십시오. 자세한 내용은 내 앱 포털 - [Azure AD의 컬렉션(미리 보기)을 참조하세요.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. 내 앱 포털에서 앱을 시작 & 앱 포털 - Azure AD에서 앱 사용 [찾기를 참조하세요.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 Mover 앱이 설치 후 Enterprise 응용 프로그램 블레이드에 표시되지 않습니다.

    "Office 365 Mover" 응용 프로그램은 앱 등록의 갤러리 응용 프로그램 섹션을 사용하여 AAD에 추가할 필요가 없는 Enterprise 앱입니다. Mover Office 365 액세스하려면 앱에 로그인하기만 하면 사용 권한에 대한 사용자의 동의를 요청합니다. 사용자가 동의하면 로그인한 전자 메일 ID를 통해 이 앱이 테넌트에 자동으로 추가됩니다.

    응용 프로그램에 로그인한 후 AAD의 Enterprise 응용 프로그램 블레이드에서 이 응용 프로그램의 항목을 찾을 수 있습니다. 전체 이름(예: "Office 365 Mover")을 입력하거나 "office"를 검색하여 해당 응용 프로그램을 검색해야 합니다. 자세한 내용은 Office 365 Mover에서 이미 설치되어 있지만 응용 프로그램 갤러리의 목록에 Enterprise [참조합니다.](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)
8. 빠른 시작: ID 관리에 [Azure Active Directory(Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) 테넌트를 사용하는 응용 프로그램 목록을 보면 Azure AD 테넌트가 ID 공급자(IdP)로 이미 설정되어 있는 응용 프로그램(앱)을 보는 방법을 보여 주게 됩니다.
9. [응용 프로그램을 추가하거나](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) 제거하는 일반적인 문제를 해결하면 Azure Active Directory 응용 프로그램에서 앱을 보는 데 직면하는 일반적인 문제를 Azure Active Directory.
