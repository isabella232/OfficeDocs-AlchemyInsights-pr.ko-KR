---
title: 자원 또는 서비스 보안 주체 관련 문제
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50716128"
---
# <a name="issues-with-a-resource-or-service-principal"></a><span data-ttu-id="cdbb0-102">자원 또는 서비스 보안 주체 관련 문제</span><span class="sxs-lookup"><span data-stu-id="cdbb0-102">Issues with a Resource or Service Principal</span></span>

1. <span data-ttu-id="cdbb0-103">방금 시작한 경우 Azure Active Directory의 응용 프로그램 및 서비스 주체 개체는 [Azure Active Directory의](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) 응용 프로그램 등록, 응용 프로그램 개체 및 서비스 주체에 대해 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="cdbb0-103">If you are just getting started, [Application and service principal objects in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span> <span data-ttu-id="cdbb0-104">응용 프로그램의 응용 프로그램 개체와 해당 서비스 사용자 개체 간의 관계를 설명하는 다중 테넌트 예제 시나리오도 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="cdbb0-104">A multi-tenant example scenario is also presented to illustrate the relationship between an application's application object and corresponding service principal objects.</span></span>
2. <span data-ttu-id="cdbb0-105">Azure Active Directory에서 응용 프로그램 및 서비스 사용자 개체를 읽어 응용 프로그램과 서비스 사용자 간의 관계에 [대해 자세히 알아보십시오.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)</span><span class="sxs-lookup"><span data-stu-id="cdbb0-105">You can learn more about the relationship between applications and service principals by reading [applications and service principal objects in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).</span></span>
3. <span data-ttu-id="cdbb0-106">[방법:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) 포털을 사용하여 리소스에 액세스할 수 있는 Azure AD 응용 프로그램 및 서비스 계정을 만들면 역할 기반 액세스 제어와 함께 사용할 수 있는 새 Azure AD(Azure Active Directory) 응용 프로그램 및 서비스 계정을 만드는 방법을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdbb0-106">[How to: Use the portal to create an Azure AD application and service principal that can access resources](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
4. <span data-ttu-id="cdbb0-107">서비스 [주체 API를](https://docs.microsoft.com/graph/api/resources/serviceprincipal)사용하여 프로그래밍식으로 응용 프로그램 인스턴스를 관리하고 응용 프로그램이 테넌트 내에서 할 수 있는 작업을 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdbb0-107">With the [service principal API](https://docs.microsoft.com/graph/api/resources/serviceprincipal), you can programmatically manage instances of applications and control what an application can do within your tenant.</span></span>
5. <span data-ttu-id="cdbb0-108">[servicePrincipal 리소스 유형에는](https://docs.microsoft.com/graph/api/resources/serviceprincipal) servicePrincipal 리소스 유형에 대한 모든 속성과 메서드가 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="cdbb0-108">[servicePrincipal resource type](https://docs.microsoft.com/graph/api/resources/serviceprincipal) lists all properties and methods for the servicePrincipal resource type.</span></span>
6. <span data-ttu-id="cdbb0-109">[Azure AD Graph와 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) 간의 리소스 유형 차이는 Azure AD Graph와 Microsoft Graph 리소스 간의 차이점을 강조합니다.</span><span class="sxs-lookup"><span data-stu-id="cdbb0-109">[Resource type differences between Azure AD Graph and Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) highlights differences between Azure AD Graph and Microsoft Graph resources.</span></span> <span data-ttu-id="cdbb0-110">이름이 다르거나 사용할 수 없는 리소스를 보여 주며, 또한 베타 버전의 Microsoft Graph에서 사용할 수 있는 리소스도 강조 표시하지만 v1.0 버전에서는 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="cdbb0-110">It shows resources that have different names or are not available; it also highlights resources available in the beta version of Microsoft Graph but not in the v1.0 version.</span></span>

<span data-ttu-id="cdbb0-111">**게스트 사용자 관련 문제**</span><span class="sxs-lookup"><span data-stu-id="cdbb0-111">**Issues with Guest Users**</span></span>

- <span data-ttu-id="cdbb0-112">[빠른 시작: Azure Portal의](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) 디렉터리에 게스트 사용자를 추가하면 Azure Portal을 통해 Azure AD 디렉터리에 새 게스트 사용자를 추가하고, 초대를 보내고, 게스트 사용자의 초대 사용 프로세스가 어떻게 보이는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdbb0-112">[Quickstart: Add guest users to your directory in the Azure portal](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) shows you how to add a new guest user to your Azure AD directory via the Azure portal, send an invitation, and see what the guest user's invitation redemption process looks like.</span></span>
- <span data-ttu-id="cdbb0-113">[자습서: Azure Active Directory B2C에서](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) 사용자 흐름 만들기는 Azure Portal을 사용하여 몇 가지 권장 사용자 흐름을 만드는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="cdbb0-113">[Tutorial: Create user flows in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) shows you how to create some recommended user flows by using the Azure portal.</span></span> <span data-ttu-id="cdbb0-114">응용 프로그램에서 리소스 소유자 암호 자격 증명(ROPC) 흐름을 설정하는 방법에 대한 자세한 내용은 Azure AD B2C에서 리소스 소유자 암호 자격 증명 흐름 구성을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cdbb0-114">If you are looking for information about how to set up a resource owner password credentials (ROPC) flow in your application, see Configure the resource owner password credentials flow in Azure AD B2C.</span></span>
