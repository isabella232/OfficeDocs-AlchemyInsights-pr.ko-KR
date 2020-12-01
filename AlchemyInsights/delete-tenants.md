---
title: 테 넌 트 삭제
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477674"
---
# <a name="delete-tenant"></a><span data-ttu-id="e3afc-102">테 넌 트 삭제</span><span class="sxs-lookup"><span data-stu-id="e3afc-102">Delete tenant</span></span>

<span data-ttu-id="e3afc-103">Azure AD를 삭제 하려면 다음을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="e3afc-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="e3afc-104">디렉터리의 전역 관리자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e3afc-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="e3afc-105">로그인 한 계정 (예: admin@contoso.onmicrosoft.com)에서 contoso.onmicrosoft.com와 같은 기본 디렉터리를 가진 계정으로 로그인 되어 있지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="e3afc-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="e3afc-106">삭제 하기 전에 디렉터리에서 활성 응용 프로그램을 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="e3afc-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="e3afc-107">활성 응용 프로그램을 제거 하려면 앱 등록으로 이동 하 여 기존 응용 프로그램을 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="e3afc-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="e3afc-108">디렉터리에 연결 된 Microsoft Azure, Office 365 또는 Azure AD Premium과 같은 Microsoft Online 서비스에 대 한 활성 구독이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="e3afc-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="e3afc-109">구독을 전송 하거나 Azure 지원 및 대금 청구를 통해 활성 구독을 신속 하 게 취소 합니다.</span><span class="sxs-lookup"><span data-stu-id="e3afc-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="e3afc-110">Office 365 및 Azure 구독을 취소 하는 방법에 대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="e3afc-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="e3afc-111">기존 구독을 테 넌 트에 연결 하거나 추가 하는 방법에 대 한 지침은 [AZURE AD 테 넌 트에 azure 구독 연결 또는 추가](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="e3afc-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="e3afc-112">활성 라이선스가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="e3afc-112">There are no Active license.</span></span> <span data-ttu-id="e3afc-113">라이선스를 제거 하려면 [라이선스 제거 구독을 제거 하는 방법을](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="e3afc-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="e3afc-114">Azure AD를 삭제 하려고 할 때 디렉터리에 다른 활성 사용자 외에는 전역 관리자로 서는 안 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e3afc-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="e3afc-115">다른 모든 활성 사용자를 제거 하 고 테 넌 트의 사용자 지정 도메인 이름에 대 한 종속성 (예: admin@contoso.com을 사용 하 여 만든 사용자)도 제거 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e3afc-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="e3afc-116">자세한 내용은 다음을 수행 하십시오.</span><span class="sxs-lookup"><span data-stu-id="e3afc-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="e3afc-117">"Azure Active Directory" 또는 "구독"을 삭제 하 고 [Azure Active Directory 삭제](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="e3afc-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="e3afc-118">디렉터리에서 응용 프로그램 제거 [응용 프로그램 제거](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app)를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="e3afc-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
