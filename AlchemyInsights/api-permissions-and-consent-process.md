---
title: API 사용 권한 및 동의 프로세스
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
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379893"
---
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="b6d32-102">API 사용 권한 및 동의 프로세스</span><span class="sxs-lookup"><span data-stu-id="b6d32-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="b6d32-103">앱에서 Microsoft Graph의 데이터에 액세스하려면 사용자 또는 관리자가 동의 프로세스를 통해 올바른 사용 권한을 부여해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b6d32-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="b6d32-104">[Microsoft Graph 사용 권한 참조에는](https://docs.microsoft.com/graph/permissions-reference) 각 주요 Microsoft Graph API 집합과 연결된 사용 권한이 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="b6d32-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="b6d32-105">또한 사용 권한을 사용하는 방법에 대한 지침도 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="b6d32-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="b6d32-106">**서비스 보안 주체 설정 또는 업데이트**</span><span class="sxs-lookup"><span data-stu-id="b6d32-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="b6d32-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - 이 문서에서는 새 servicePrincipal 개체를 만드는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="b6d32-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="b6d32-108">[포털에서 Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) 앱 & 서비스 사용자 만들기 - 이 문서에서는 역할 기반 액세스 제어와 함께 사용할 수 있는 새 Azure AD(Azure Active Directory) 응용 프로그램 및 서비스 계정을 만드는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="b6d32-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="b6d32-109">[Azure AD의](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) & 앱 - 이 문서에서는 Azure Active Directory의 응용 프로그램 등록, 응용 프로그램 개체 및 서비스 주체에 대해 설명합니다. 이 문서에서는 응용 프로그램 등록, 응용 프로그램 개체 및 서비스 주체의 대상, 사용 방법 및 서로의 관계에 대해 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="b6d32-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="b6d32-110">**앱 등록 추가 또는 업데이트 및 관리자 동의 제공**</span><span class="sxs-lookup"><span data-stu-id="b6d32-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="b6d32-111">[앱 등록 만들기](https://docs.microsoft.com/graph/api/application-post-applications) - 이 문서에서는 새 응용 프로그램 개체를 만드는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="b6d32-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="b6d32-112">[앱 등록 업데이트 - API 권한](https://docs.microsoft.com/graph/api/application-update) - 이 문서에서는 응용 프로그램 개체의 속성을 업데이트하는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="b6d32-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="b6d32-113">[관리자 동의 제공](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - 일반적으로 관리자 동의 및 동의를 위해서는 관리자가 명시적으로 동의를 부여해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b6d32-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="b6d32-114">[RBAC(베타)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - 단일 역할 할당에서 여러 사용자 및 여러 범위를 지원하는 Microsoft 365 RBAC 공급자에 대한 통합 역할 정의 및 역할 할당에 대한 역할 관리 컨테이너입니다.</span><span class="sxs-lookup"><span data-stu-id="b6d32-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="b6d32-115">이는 *rbacApplication* 리소스 유형과 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="b6d32-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="b6d32-116">Microsoft Intune은 이러한 RBAC 공급자의 예입니다.</span><span class="sxs-lookup"><span data-stu-id="b6d32-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="b6d32-117">Intune의 역할 할당에는 보안 주체 배열과 범위 그룹 배열이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b6d32-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="b6d32-118">**베타 버전이며, 이는 아직 개발 중이며 프로덕션에서 사용하기에 권장되지 않음을 의미합니다.**</span><span class="sxs-lookup"><span data-stu-id="b6d32-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>
