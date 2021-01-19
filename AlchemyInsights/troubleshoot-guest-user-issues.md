---
title: 게스트 사용자 문제 해결
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897747"
---
# <a name="troubleshoot-guest-user-issues"></a><span data-ttu-id="44262-102">게스트 사용자 문제 해결</span><span class="sxs-lookup"><span data-stu-id="44262-102">Troubleshoot guest user issues</span></span>

1. <span data-ttu-id="44262-103">응용 프로그램에 대한 게스트 액세스 관리에 대한 지침은 Azure AD 액세스 검토를 사용하여 게스트 [액세스 관리를 참조하세요.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)</span><span class="sxs-lookup"><span data-stu-id="44262-103">For guidance on managing guest access to applications, see [Manage guest access with Azure AD access reviews](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).</span></span>
1. <span data-ttu-id="44262-104">[Azure Portal의](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)디렉터리에 게스트 사용자를 추가합니다. 이 빠른 시작에서는 Azure Portal을 통해 Azure AD 디렉터리에 새 게스트 사용자를 추가하고 초대를 보내며 게스트 사용자의 초대 중복 프로세스 모양을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="44262-104">[Add guest users to your directory in the Azure portal](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): In this quickstart, you'll add a new guest user to your Azure AD directory via the Azure portal, send an invitation, and see what the guest user's invitation redemption process looks like.</span></span>
1. <span data-ttu-id="44262-105">[PowerShell을](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)사용하여 게스트 사용자 추가: 이 빠른 시작에서는 New-AzureADMSInvitation 명령을 사용하여 Azure 테넌트에 게스트 사용자를 하나 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="44262-105">[Add a guest user with PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): In this quickstart, you’ll use the New-AzureADMSInvitation command to add one guest user to your Azure tenant.</span></span>
1. <span data-ttu-id="44262-106">Azure Portal 내에서 또는 PowerShell을 사용하여 Azure AD(Azure Active Directory)의 엔터프라이즈 응용 프로그램에 사용자 및 그룹을 할당하는 방법에 대한 자세한 내용은 [Azure Active Directory에서](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)앱에 대한 사용자 할당 관리를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="44262-106">To learn how to assign users, and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span> 
1. <span data-ttu-id="44262-107">Azure AD(Azure Active Directory) B2B 공동 작업은 Azure AD와 통합되는 대부분의 앱에서 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="44262-107">Azure Active Directory (Azure AD) B2B collaboration works with most apps that integrate with Azure AD.</span></span> <span data-ttu-id="44262-108">이 [문서에서는](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)Azure AD B2B에서 사용할 수 있는 몇 가지 인기 있는 SaaS 앱을 구성하기 위한 지침을 안내합니다.</span><span class="sxs-lookup"><span data-stu-id="44262-108">In this [article](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps), we walk through instructions for configuring some popular SaaS apps for use with Azure AD B2B.</span></span>
1. <span data-ttu-id="44262-109">Azure AD(Azure Active Directory) B2B 공동 작업 기능을 사용하여 파트너 조직의 게스트 사용자를 Azure AD로 초대하는 조직은 이제 이러한 B2B 사용자에게 해당 B2B 사용자에 대한 액세스 권한을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="44262-109">As an organization that uses Azure Active Directory (Azure AD) B2B collaboration capabilities to invite guest users from partner organizations to your Azure AD, you can now provide these B2B users access to on-premises apps.</span></span> <span data-ttu-id="44262-110">이러한 On-premises 앱은 SAML 기반 인증 또는 Kerberos KCD(제한 위임)와 함께 IWA(Windows 통합 인증)를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="44262-110">These on-premises apps can use SAML-based authentication or Integrated Windows Authentication (IWA) with Kerberos constrained delegation (KCD).</span></span> <span data-ttu-id="44262-111">자세한 내용은 Azure [AD에서 B2B 사용자에게 On-premises](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)응용 프로그램에 대한 액세스 권한 부여를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="44262-111">For more information, see [Grant B2B users in Azure AD access to your on-premises applications](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).</span></span>
1. <span data-ttu-id="44262-112">[Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)공동 작업을 사용하여 로컬 관리 파트너 계정에 클라우드 리소스에 대한 액세스 권한을 부여하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="44262-112">Learn how to [grant locally-managed partner accounts access to cloud resources using Azure AD B2B collaboration](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).</span></span>