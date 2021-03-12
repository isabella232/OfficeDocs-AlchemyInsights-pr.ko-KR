---
title: 그룹 문제 해결
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
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "50716110"
---
# <a name="troubleshoot-group-issues"></a><span data-ttu-id="c564e-102">그룹 문제 해결</span><span class="sxs-lookup"><span data-stu-id="c564e-102">Troubleshoot group issues</span></span>

<span data-ttu-id="c564e-103">**Azure AD 역할에 그룹을 할당해야 하는 경우**</span><span class="sxs-lookup"><span data-stu-id="c564e-103">**I need to assign a group to an Azure AD role**</span></span>

<span data-ttu-id="c564e-104">Azure AD 역할에 Azure AD(Active Directory) 그룹을 할당하는 경우 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-104">To assign an Azure Active Directory (AD) group to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="c564e-105">새 그룹 만들기-새 그룹을 만들려면 :</span><span class="sxs-lookup"><span data-stu-id="c564e-105">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="c564e-106">a.</span><span class="sxs-lookup"><span data-stu-id="c564e-106">a.</span></span> <span data-ttu-id="c564e-107">권한 있는 역할 관리자 또는 전역 관리자 권한으로 Azure AD 관리 센터에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-107">Sign in to the Azure AD admin center with privileged role administrator or global administrator permissions.</span></span> 
    <span data-ttu-id="c564e-108">b.</span><span class="sxs-lookup"><span data-stu-id="c564e-108">b.</span></span> <span data-ttu-id="c564e-109">Azure Active Directory> 그룹> 모든 그룹> 새 그룹을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-109">Select Azure Active Directory > Groups > All groups > New group.</span></span> 
    <span data-ttu-id="c564e-110">c.</span><span class="sxs-lookup"><span data-stu-id="c564e-110">c.</span></span> <span data-ttu-id="c564e-111">그룹을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-111">Create the group.</span></span>

2. <span data-ttu-id="c564e-112">그룹을 만드는 동안 또는 그룹을 만든 후에 역할을 그룹에 할당합니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-112">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="c564e-113">a.</span><span class="sxs-lookup"><span data-stu-id="c564e-113">a.</span></span> <span data-ttu-id="c564e-114">그룹 생성시 그룹에 역할을 할당하려면 Azure AD 역할을 그룹에 할당할 수 있음 토글을 켜고 그룹을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-114">To assign a role to the group at the time of group creation, switch on the toggle Azure AD roles can be assigned to the group and create the group.</span></span>
    <span data-ttu-id="c564e-115">b.</span><span class="sxs-lookup"><span data-stu-id="c564e-115">b.</span></span> <span data-ttu-id="c564e-116">그룹을 만든 후 그룹에 역할을 할당하려면 새로 만든 그룹의 할당된 역할 탭으로 이동하여 그룹에 역할을 할당합니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-116">To assign a role to the group after it has been created, navigate to the Assigned roles tab for the newly created group, and assign the role to the group.</span></span>

<span data-ttu-id="c564e-117">**Azure AD 역할에 할당된 그룹의 구성원 자격을 관리해야 하는 경우**</span><span class="sxs-lookup"><span data-stu-id="c564e-117">**I need to manage membership of a group that is assigned to Azure AD role**</span></span>

1. <span data-ttu-id="c564e-118">권한 상승을 방지하기 위해 기본적으로 권한 있는 역할 관리자와 전역 관리자만 역할에 할당된 그룹의 구성원 자격을 수정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-118">To prevent elevation of privileges, by default, only privileged role administrator and global administrator can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="c564e-119">그러나 이러한 그룹에 대한 소유자를 지정하고 이 작업을 대리하도록 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-119">They can, however, choose to assign an owner for such a group and delegate this task.</span></span> <span data-ttu-id="c564e-120">자세한 내용은 [Azure Active Directory에서 클라우드 그룹을 사용하여 역할 할당](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c564e-120">For more information see, [Use cloud groups to manage role assignments in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span>
2. <span data-ttu-id="c564e-121">Azure AD의 그룹에 역할을 할당하기 위한 일반적인 질문과 문제 해결 팁은 [클라우드 그룹에 할당된 역할 문제 해결](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c564e-121">For common questions and troubleshooting tips for assigning roles to groups in Azure AD, see [Troubleshooting roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>

<span data-ttu-id="c564e-122">**동적 그룹**</span><span class="sxs-lookup"><span data-stu-id="c564e-122">**Dynamic groups**</span></span>

1. <span data-ttu-id="c564e-123">기본 제공 사용자 특성을 찾을 수 없는 경우 이 특성이 지원되는 속성 목록에 나열되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-123">If you cannot find the built-in user attributes, ensure that the attribute is in the list of supported properties.</span></span>
2. <span data-ttu-id="c564e-124">기본 제공 장치 특성을 찾고 있는 경우 특성이 장치 특성 목록에 표시되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-124">If you are looking for built-in device attributes, ensure that the attribute is in the list of device attributes</span></span> 
3. <span data-ttu-id="c564e-125">기본 제공 사용자 및 장치 특성 외에도 [확장 특성](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties)도 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-125">In addition to the built-in user and device attributes, you could also use [Extension Attributes](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties).</span></span> <span data-ttu-id="c564e-126">확장 특성을 온-프레미스 Windows Server AD 또는 연결된 SaaS 응용 프로그램에서 동기화하면 규칙 작성기 드롭다운 목록에 특성이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-126">After syncing extension attributes from on-premises Windows Server AD or from a connected SaaS application, the attributes should be visible in the drop-down list of the rule builder.</span></span> <span data-ttu-id="c564e-127">PowerShell을 사용하여 사용자 특성을 쿼리하고 특성 이름을 검색하여 사용자 지정 특성 이름을 디렉터리에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-127">The custom attribute name can be found in the directory by querying a user's attribute using PowerShell and searching for the attribute name.</span></span> <span data-ttu-id="c564e-128">규칙 구문에서 규칙을 구성할 때도 이러한 규칙을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-128">These could also be used when constructing rules in the rule syntax.</span></span>
4. <span data-ttu-id="c564e-129">테넌트에 적절한 라이선스가 부여되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-129">Ensure that your tenant has the appropriate license.</span></span> <span data-ttu-id="c564e-130">동적 그룹을 사용하려면 테넌트에 Azure AD P1 Premium 라이선스가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-130">Dynamic groups require the tenant to have an Azure AD P1 Premium license.</span></span> <span data-ttu-id="c564e-131">[여기](https://azure.microsoft.com/pricing/details/active-directory/)에서 Azure AD 라이선스 계획 목록에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-131">The list of Azure AD license plans can be accessed [here](https://azure.microsoft.com/pricing/details/active-directory/).</span></span> <span data-ttu-id="c564e-132">Enterprise Mobility + Security 라이선스 계획은 [여기](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)에서 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-132">Enterprise Mobility + Security licensing plans can be accessed [here](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).</span></span>
5. <span data-ttu-id="c564e-133">동적 그룹을 만드는 사용자의 역할이 전역 관리자, intune 관리자, 그룹 관리자 또는 사용자 관리자인지 합니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-133">Ensure that the role of the user creating the dynamic group is a global administrator, intune administrator, group administrator, or a user administrator.</span></span>
6. <span data-ttu-id="c564e-134">그룹이 채워질 시간을 충분히 줍니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-134">Please allow time for the group to populate.</span></span> <span data-ttu-id="c564e-135">그룹은 테넌트의 크기에 따라 처음 또는 규칙 변경 후 채우는 데 최대 24시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-135">Depending on the size of your tenant, the group may take up to 24 hours for populating for the first time or after a rule change.</span></span>
7. <span data-ttu-id="c564e-136">자세한 내용은 [그룹 구성원 자격에 대한 특성 기반 규칙 만들기](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c564e-136">For more information, see [Create attribute-based rules for dynamic group membership](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).</span></span>

<span data-ttu-id="c564e-137">**그룹을 삭제해야 하는 경우**</span><span class="sxs-lookup"><span data-stu-id="c564e-137">**I need to delete a group**</span></span>

1. <span data-ttu-id="c564e-138">Azure AD PowerShell 모듈의 Remove-AzureADGroup cmdlet을 사용하여 디렉터리에서 그룹을 삭제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-138">Groups can be deleted from the directory using the Remove-AzureADGroup cmdlet in the Azure AD Powershell module.</span></span>
2. <span data-ttu-id="c564e-139">Azure AD에서 동기화된 그룹을 삭제하기 전에 먼저 오류 발생을 방지하기 위해 할당된 모든 라이선스를 삭제했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-139">Before attempting to delete a synced group in Azure AD, ensure you have deleted all assigned licenses  to avoid errors.</span></span>
3. <span data-ttu-id="c564e-140">그룹 삭제에 대한 자세한 내용은 [할당된 라이선스가 할당된 그룹 삭제](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c564e-140">For more information on deleting groups, see [Deleting a group with an assigned license](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).</span></span>

<span data-ttu-id="c564e-141">**삭제된 그룹을 복원해야 하는 경우**</span><span class="sxs-lookup"><span data-stu-id="c564e-141">**I need to restore a deleted group**</span></span>

1. <span data-ttu-id="c564e-142">Office 365 그룹이 삭제된 경우 영구 삭제가 발생하기 최대 30일 전까지만 복원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-142">If an Office 365 group is deleted, it can only be restored up to 30 days before permanent deletion occurs.</span></span> <span data-ttu-id="c564e-143">영구적으로 삭제된 그룹은 더 이상 복원할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-143">Once permanently deleted, the group can no longer be restored.</span></span> <span data-ttu-id="c564e-144">[여기](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)에서 그룹 복원에 대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="c564e-144">Learn more about restoring groups [here](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>
2. <span data-ttu-id="c564e-145">이 기능은 보안 그룹 및 메일 그룹에서 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-145">This functionality is not supported for security groups and distribution groups.</span></span>
3. <span data-ttu-id="c564e-146">Office 365 그룹을 복원할 권한이 부여되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-146">Ensure you are authorized to restore an Office 365 group.</span></span> <span data-ttu-id="c564e-147">전역 관리자, 그룹 관리자, 사용자 계정 관리자, intune 서비스 관리자, 파트너 티어 1 또는 티어 2 지원 및 그룹 소유자는 그룹을 복원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-147">Global administrators, group administrators, user account administrators, intune service administrators, partner tier1 or tier2 support, and the owner of the group can be able to restore a group.</span></span>
4. <span data-ttu-id="c564e-148">동적 그룹이 삭제 및 복원되면 해당 그룹이 새 그룹으로 표시되고 규칙에 따라 다시 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-148">When a dynamic group is deleted and restored, it is seen as a new group and re-populated according to the rule.</span></span> <span data-ttu-id="c564e-149">이 프로세스는 최대 24시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-149">This process might take up to 24 hours.</span></span>
5. <span data-ttu-id="c564e-150">삭제된 그룹 복원에 대한 자세한 내용은 [Azure Active Directory에서 삭제된 Office 365 그룹 복원](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c564e-150">For more information on restoring a deleted group, see [Restore a deleted Office 365 group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="c564e-151">**그룹 만료 정책 구성**</span><span class="sxs-lookup"><span data-stu-id="c564e-151">**Group expiration policy configuration**</span></span>

1. <span data-ttu-id="c564e-152">이 기능은 Office 365 그룹에만 지원될 뿐, 보안 그룹 및 메일 그룹에는 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-152">This functionality is only supported for Office 365 groups, and not for security groups and distribution groups are not supported.</span></span>
2. <span data-ttu-id="c564e-153">Office 365 그룹의 만료 정책을 구성하고 사용하려면 Azure AD Premium 라이선스가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-153">Configuring and using the expiration policy for Office 365 groups requires an Azure AD Premium license.</span></span>
3. <span data-ttu-id="c564e-154">현재 테넌트의 Office 365 그룹에 대해 하나의 만료 정책만 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-154">Currently, only one expiration policy can be configured for Office 365 groups on a tenant.</span></span>
4. <span data-ttu-id="c564e-155">전역 관리자, 그룹 관리자, 사용자 관리자 및 그룹의 소유자만 그룹을 갱신할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-155">Only Global administrators, group administrators, user administrators, and the owner of the group can be able to renew a group.</span></span>
5. <span data-ttu-id="c564e-156">Office 365 그룹이 만료된 경우, 해당 그룹은 삭제되며 영구 삭제가 발생하기 최대 30일 전까지만 복원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-156">If an Office 365 group is expired, it is deleted and can only be restored up to 30 days before permanent deletion occurs.</span></span> <span data-ttu-id="c564e-157">영구적으로 삭제된 그룹은 더 이상 복원할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-157">Once permanently deleted, the group can no longer be restored.</span></span> <span data-ttu-id="c564e-158">[여기](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)에서 그룹 복원에 대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="c564e-158">Learn more about restoring groups [here](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="c564e-159">**활동 기반 자동 갱신**</span><span class="sxs-lookup"><span data-stu-id="c564e-159">**Activity-based automatic renewal**</span></span>

<span data-ttu-id="c564e-160">SharePoint, Outlook 및 Teams의 사용자 활동은 그룹 자동 갱신을 트리거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-160">User activities from SharePoint, Outlook and Teams can trigger group automatic renewal.</span></span> <span data-ttu-id="c564e-161">활동은 그룹이 만료되기 35일 전에 검사됩니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-161">Activities are checked at 35 days before a group expires.</span></span> <span data-ttu-id="c564e-162">현재 그룹 수명 주기 동안 활동이 있는 경우 그룹이 자동으로 갱신되고 그룹 소유자에게 전자 메일 알림이 전송되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-162">If there is activity during the current group lifecycle, the group will be automatically renewed and email notification won't be sent out to group owners.</span></span>

<span data-ttu-id="c564e-163">**만료된 그룹의 알림 타이밍**</span><span class="sxs-lookup"><span data-stu-id="c564e-163">**Notification timing for expired groups**</span></span>

1. <span data-ttu-id="c564e-164">전자 메일 알림은 그룹 만료 30일, 15일 및 1일 전에 Office 365 그룹 소유자에게 전송됩니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-164">Email notifications are sent to the Office 365 group owners 30 days, 15 days, and 1 day prior to expiration of the group.</span></span>
2. <span data-ttu-id="c564e-165">처음 만료를 설정할 때 만료 간격보다 오래된 그룹은 만료까지 35일로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-165">When you first set up expiration, any groups that are older than the expiration interval are set to 35 days until expiration.</span></span>
3. <span data-ttu-id="c564e-166">그룹 만료 날짜는 정책 업데이트 날짜가 아니라 그룹의 갱신 날짜를 기준으로 계산됩니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-166">Group expiration date is calculated based on the group’s renewal date, not based on the policy updated date.</span></span> <span data-ttu-id="c564e-167">만료 정책이 업데이트되는 경우 만료 날짜는 변경되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-167">If the expiration policy is updated, the expiration date will not change.</span></span>
4. <span data-ttu-id="c564e-168">자세한 내용은 [그룹 만료 정책 및 갱신 전자 메일](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) 및 [Azure Active Directory 365에서 삭제된 Office 365 그룹 복원](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c564e-168">For more information see, [Group Expiration policy and renewal emails](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) and [Restore a deleted Office 365 group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="c564e-169">**그룹을 만들 수 있는 권한**</span><span class="sxs-lookup"><span data-stu-id="c564e-169">**Permission to create a group**</span></span>

<span data-ttu-id="c564e-170">새 그룹을 만들 수 있는 권한을 부여받았는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-170">Ensure that you are authorized to create a new group.</span></span> <span data-ttu-id="c564e-171">전역 관리자는 Azure 포털 또는 액세스 패널에서 그룹 만들기를 사용하지 않도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-171">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="c564e-172">관리자가 새 그룹을 만들거나 적절한 사용 권한을 부여해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-172">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

1. [<span data-ttu-id="c564e-173">Azure Portal에서 새 그룹 만들기 및 구성원 추가</span><span class="sxs-lookup"><span data-stu-id="c564e-173">Create a new group and add members in Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [<span data-ttu-id="c564e-174">PowerShell MSOnline에서 그룹 만들기</span><span class="sxs-lookup"><span data-stu-id="c564e-174">Create groups in Powershell MSOnline</span></span>](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [<span data-ttu-id="c564e-175">PowerShell에서 그룹 만들기 사용 해제</span><span class="sxs-lookup"><span data-stu-id="c564e-175">Disable groups creation in Powershell</span></span>](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [<span data-ttu-id="c564e-176">Office 365에서 그룹을 만들 수 있는 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="c564e-176">Manage who can create groups in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [<span data-ttu-id="c564e-177">Powershell을 통해 Office 365 시작 알림 사용 해제</span><span class="sxs-lookup"><span data-stu-id="c564e-177">Disable Office 365 welcome notification via Powershell</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [<span data-ttu-id="c564e-178">Azure AD 관리 역할</span><span class="sxs-lookup"><span data-stu-id="c564e-178">Azure AD administrative roles</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

<span data-ttu-id="c564e-179">**그룹 만들기 권한 관리**</span><span class="sxs-lookup"><span data-stu-id="c564e-179">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="c564e-180">전역 관리자는 **사용자가 Azure Portal에서 보안 그룹을 만들 수 있음** 또는 **사용자가 **모든 그룹> 일반(설정)** 의 Azure Portal 설정에서 Office 365 그룹을 만들 수 있음** 을 설정하여 Azure Portal 또는 액세스 패널에서 만든 보안 또는 Office 365 그룹에 대한 그룹 만들기 권한을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-180">Global administrators can manage group creation permissions for security or Office 365 groups created in the Azure portal or Access Panel, by setting **Users can create security groups in Azure portals** or **Users can create Office 365 groups in Azure portals** settings in **All groups > General (Settings)**.</span></span>
2. <span data-ttu-id="c564e-181">Azure AD P1 Premium 라이선스가 있는 경우 그룹 만들기를 제한하여 사용자 그룹을 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-181">You can also restrict group creation to select a group of users if you have an Azure AD P1 Premium license.</span></span>

<span data-ttu-id="c564e-182">**Office 365 그룹의 새 구성원에 대해 시작 알림 사용 해제**</span><span class="sxs-lookup"><span data-stu-id="c564e-182">**Disabling welcome notification for new members of an Office 365 group**</span></span>

<span data-ttu-id="c564e-183">Office 365 그룹에 추가된 사용자에게 전송되는 환영 알림은 Powershell에서 `UnifiedGroupWelcomeMessageEnabled`을(를) **거짓** 으로 설정하여 사용 해제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c564e-183">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting `UnifiedGroupWelcomeMessageEnabled` to **False** in Powershell.</span></span> <span data-ttu-id="c564e-184">[여기](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)에서 이 설정에 대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="c564e-184">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).</span></span>













