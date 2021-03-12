---
title: 테넌트 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7824"
- "9004325"
ms.openlocfilehash: 43f75564667bbb952076d4c12d7a1dd1e7e99731
ms.sourcegitcommit: 4e2d640a618c786700e8b276533554d51956f080
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50716164"
---
# <a name="issues-with-tenants"></a><span data-ttu-id="e420f-102">테넌트 문제</span><span class="sxs-lookup"><span data-stu-id="e420f-102">Issues with tenants</span></span>

<span data-ttu-id="e420f-103">Azure AD(Azure Active Directory)는 사용자 및 앱과 같은 개체를 테넌트라는 그룹으로 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="e420f-103">Azure Active Directory (Azure AD) organizes objects like users and apps into groups called tenants.</span></span> <span data-ttu-id="e420f-104">테넌트에서는 관리자가 조직 내의 사용자 및 조직이 소유한 앱에 대한 정책을 설정하여 보안 및 운영 정책을 충족할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e420f-104">Tenants allow an administrator to set policies on the users within the organization and the on apps that the organization owns to meet their security and operational policies.</span></span> <span data-ttu-id="e420f-105">자세한 내용은 [Azure Active Directory의 테넌시](https://docs.microsoft.com/azure/active-directory/develop/single-and-multi-tenant-apps)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e420f-105">For more information, see [Tenancy in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/single-and-multi-tenant-apps).</span></span>

<span data-ttu-id="e420f-106">테넌트 관리와 관련된 자세한 내용은 다음 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e420f-106">For more information related to tenant management, see the following articles:</span></span>

- <span data-ttu-id="e420f-107">[Quickstart: 테넌트 설정](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant) - 새 테넌트를 만드는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="e420f-107">[Quickstart: Set up a tenant](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant) - Shows you how to create a new tenant.</span></span>

- <span data-ttu-id="e420f-108">[Azure Active Directory에서 테넌트 삭제](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto) - 테넌트를 삭제하는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="e420f-108">[Delete a tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto) - Shows you how to delete a tenant.</span></span>

<span data-ttu-id="e420f-109">**다중 테넌트 문제**</span><span class="sxs-lookup"><span data-stu-id="e420f-109">**Issues with multi-tenants**</span></span>

<span data-ttu-id="e420f-110">다중 테넌트와 관련된 문제를 관리하는 방법에 대한 자세한 내용은 다음 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e420f-110">For information on how to manage issues regarding multi-tenants, see the following articles:</span></span>

- <span data-ttu-id="e420f-111">[방법: 다중 테넌트 응용 프로그램 패턴을 사용하여 Azure Active Directory 사용자로 로그인](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant) - 단일 테넌트에서 다중 테넌트 응용 프로그램으로 변환하는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="e420f-111">[How to: Sign in any Azure Active Directory user using the multi-tenant application pattern](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant) - Shows you how to convert from a single-tenant to a multi-tenant application.</span></span>
- <span data-ttu-id="e420f-112">[Azure Active Directory B2C에서 특정 Azure Active Directory 조직에 대한 로그인 설정](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-single-tenant?pivots=b2c-user-flow) - Azure AD B2C의 사용자 흐름을 사용하여 특정 Azure AD 조직의 사용자에 대해 로그인을 사용하도록 설정하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="e420f-112">[Set up sign-in for a specific Azure Active Directory organization in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-single-tenant?pivots=b2c-user-flow) - Shows you how to enable sign-in for users from a specific Azure AD organization using a user flow in Azure AD B2C.</span></span>
- <span data-ttu-id="e420f-113">[Azure Active Directory B2C에서 사용자 지정 정책을 사용하여 다중 테넌트 Azure Active Directory에 대한 로그인 설정](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-multi-tenant?pivots=b2c-custom-policy)  Azure AD(Azure Active Directory)의 다중 테넌트 끝점을 사용하여 사용자에 대해 로그인을 사용하도록 설정하는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="e420f-113">[Set up sign-in for multi-tenant Azure Active Directory using custom policies in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-multi-tenant?pivots=b2c-custom-policy)  shows you how to enable sign-in for users using the multi-tenant endpoint for Azure Active Directory (Azure AD).</span></span>






