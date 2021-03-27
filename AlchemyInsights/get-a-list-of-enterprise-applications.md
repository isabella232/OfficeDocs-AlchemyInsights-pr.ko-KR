---
title: 엔터프라이즈 응용 프로그램 목록 표시
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
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379916"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="fe609-102">엔터프라이즈 응용 프로그램 목록 표시</span><span class="sxs-lookup"><span data-stu-id="fe609-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="fe609-103">Powershell 명령을 통해 엔터프라이즈 응용 프로그램(모든 응용 프로그램 또는 표시 이름, ID, 식별자 URIS 등으로 필터링)의 목록을 얻거나 [Get-AzureADApplication (AzureAD)을](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)참조하세요. </span><span class="sxs-lookup"><span data-stu-id="fe609-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="fe609-104">Powershell 명령을 통해 서비스 사용자 개체(모든 개체 또는 ID로 필터링된 개체) 목록을 얻하려면 [Get-AzureADServicePrincipal (AzureAD)를](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)참조하세요.</span><span class="sxs-lookup"><span data-stu-id="fe609-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="fe609-105">SAML로 구성된 앱 목록을 얻게 하려는 경우 **PowerShell** 스크립트를 따라 다음 작업을 하는 것이 도움이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="fe609-106">모든 응용 프로그램이 OAuth 앱 또는 SAML 앱(갤러리 앱과 갤러리 앱이 아닌 앱 모두)이면 등록이 진행될 때 AAD에서 두 개의 개체가 만들어집니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="fe609-107">하나는 Application 개체라고, 다른 하나는 Service Principal 개체입니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="fe609-108">PowerShell을 사용하여 서비스 사용자 개체의 속성을 덤프하면 모든 응용 프로그램에 특정 수의 태그가 연결되어 있는 것을 발견할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="fe609-109">OAuth 앱에는 **"WindowsAzureActiveDirectoryIntegratedApp" 태그가 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="fe609-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="fe609-110">갤러리 SAML 앱에는 **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1"** 태그가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="fe609-111">갤러리가 아닌 SAML 앱에는 **"WindowsAzureActiveDirectoryCustomSingleSignOnApplication" 태그가 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="fe609-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="fe609-112">따라서 이러한 태그를 사용하여 앱의 종류를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="fe609-113">**"WindowsAzureActiveDirectoryIntegratedApp"** 태그는 모든 유형의 앱에서 일반적입니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="fe609-114">다음 코드 코드 일부를 사용하여 모든 SAML 앱(갤러리와 갤러리가 아닌 앱 모두)을 나열할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="fe609-115">자세한 내용은 [Azure AD에서 SAML 사용 앱 식별을 참조하세요.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="fe609-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="fe609-116">**웹 응용 프로그램만** 찾아서 나열: 다음 명령을 사용하여 응용 프로그램 유형이 "Web app/API"인 모든 Azure AD 응용 프로그램을 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="fe609-117">Get-AzureADApplication -All:$true | Where-Object { $_를 사용합니다. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="fe609-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="fe609-118">**네이티브 응용 프로그램만 찾아서** 나열: 다음 명령을 실행하여 모든 기본 클라이언트(데스크톱/모바일 장치) 응용 프로그램을 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="fe609-119">Get-AzureADApplication -All:$true | Where-Object { $_를 사용합니다. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="fe609-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="fe609-120">등록된 모든 Azure AD 응용 프로그램 세부 정보를 **CSV로** 내보내기: 아래 명령은 필요한 세부 정보가 있는 모든 Azure AD 앱을 csv 파일로 내보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="fe609-121">Get-AzureADApplication -All:$true | Select-Object, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="fe609-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="fe609-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="fe609-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="fe609-123">사용되지 않는 Azure 앱 목록을 **내보내야 합니다.** – 감사 보고서</span><span class="sxs-lookup"><span data-stu-id="fe609-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="fe609-124">Azure AD Premium 라이선스가 있는 경우 Azure AD는 최대 30일 동안만 응용 프로그램 로그를 표시할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="fe609-125">데이터를 30일 이상 보존하는 두 가지 옵션이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="fe609-126">Azure AD [보고 API를](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) 사용하여 프로그래밍식으로 데이터를 검색하고 데이터베이스에 저장할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="fe609-127">또는 감사 로그를 타사 SIEM 시스템에 통합할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="fe609-128">또한 모든 응용 프로그램 및 소유 응용 프로그램에 대한 앱 목록을 Azure Active Directory>앱 등록에서 모든 응용 프로그램/소유 응용>>다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe609-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="fe609-129">MS Graph를 통해 응용 프로그램 목록을 얻었다면 목록 응용 프로그램 [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) 및 응용 프로그램 리소스 [유형 - Microsoft Graph v1.0을 참조하세요.](https://docs.microsoft.com/graph/api/resources/application)</span><span class="sxs-lookup"><span data-stu-id="fe609-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
