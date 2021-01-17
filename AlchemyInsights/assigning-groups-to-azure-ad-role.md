---
title: Azure AD 역할에 그룹 할당
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49875406"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="6497f-102">Azure AD 역할에 그룹 할당</span><span class="sxs-lookup"><span data-stu-id="6497f-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="6497f-103">Azure AD의 권한 소스가 있는 Azure AD 그룹을 Azure AD 역할에 할당하려면 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="6497f-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="6497f-104">새 그룹 만들기-새 그룹을 만들려면 :</span><span class="sxs-lookup"><span data-stu-id="6497f-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="6497f-105">a.</span><span class="sxs-lookup"><span data-stu-id="6497f-105">a.</span></span> <span data-ttu-id="6497f-106">**권한 있는 역할 관리자** 또는 **전역 관리자** 권한으로 Azure AD 관리 센터에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="6497f-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="6497f-107">b.</span><span class="sxs-lookup"><span data-stu-id="6497f-107">b.</span></span> <span data-ttu-id="6497f-108">**Azure Active Directory> 그룹> 모든 그룹> 새 그룹** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="6497f-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="6497f-109">c.</span><span class="sxs-lookup"><span data-stu-id="6497f-109">c.</span></span> <span data-ttu-id="6497f-110">그룹을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="6497f-110">Create the group.</span></span>

2. <span data-ttu-id="6497f-111">그룹을 만드는 동안 또는 그룹을 만든 후에 역할을 그룹에 할당합니다.</span><span class="sxs-lookup"><span data-stu-id="6497f-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="6497f-112">a.</span><span class="sxs-lookup"><span data-stu-id="6497f-112">a.</span></span> <span data-ttu-id="6497f-113">그룹 생성시 그룹에 역할을 할당하려면 **Azure AD 역할을 그룹에 할당할 수 있음** 토글을 켜고 그룹을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="6497f-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="6497f-114">b.</span><span class="sxs-lookup"><span data-stu-id="6497f-114">b.</span></span> <span data-ttu-id="6497f-115">그룹을 만든 후 그룹에 역할을 할당하려면 새로 만든 그룹의 **할당된 역할** 탭으로 이동하여 그룹에 역할을 할당합니다.</span><span class="sxs-lookup"><span data-stu-id="6497f-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="6497f-116">**Azure AD 역할에 할당 된 그룹의 구성원 관리**</span><span class="sxs-lookup"><span data-stu-id="6497f-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="6497f-117">권한 상승을 방지하기 위해 기본적으로 권한 있는 역할 관리자와 전역 관리자만 역할에 할당된 그룹의 구성원 자격을 수정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6497f-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="6497f-118">그러나 이러한 그룹에 대한 소유자를 지정하고 이 작업을 대리하도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6497f-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="6497f-119">클라우드 그룹을 Azure AD 역할에 할당하는 방법에 대한 자세한 내용은 [클라우드 그룹에 AD 역할 할당](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6497f-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="6497f-120">클라우드 그룹에 할당된 역할 문제 해결에 대한 자세한 내용은 [클라우드 그룹에 할당된 역할 문제 해결 ](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6497f-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





