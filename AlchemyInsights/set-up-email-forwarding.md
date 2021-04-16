---
title: 전자 메일 전달 설정
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "20"
- "1200004"
ms.assetid: 15abf81d-5c5d-49da-ac81-1b4daa1809f6
ms.openlocfilehash: a7fba259375c667ff2e0f14a03972e102468cd27
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51787143"
---
# <a name="check-the-email-forwarding-settings-for-a-mailbox"></a><span data-ttu-id="c6697-102">사서함에 대한 전자 메일 전달 설정 확인</span><span class="sxs-lookup"><span data-stu-id="c6697-102">Check the email forwarding settings for a mailbox</span></span>

<span data-ttu-id="c6697-103">첫째, 테넌트 수준에서 전자 메일 전달을 사용하도록 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6697-103">Firstly, email forwarding has to be enabled on the tenant level.</span></span> <span data-ttu-id="c6697-104">사서함에 전자 메일 전달을 설정했지만 작동하지 않는 **경우("550 5.7.520 액세스 거부,** 조직에서 외부 전달을 허용하지 않습니다."라는 오류가 표시) [Microsoft 365에서](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide)자동 외부 전자 메일 전달 제어를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c6697-104">If you have set up email forwarding on a mailbox, but it is not working (you get an error **"550 5.7.520 Access denied, Your organization does not allow external forwarding"**) please see [Control automatic external email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide).</span></span>

<span data-ttu-id="c6697-105">사서함에서 전자 메일 전달 설정을 쉽게 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c6697-105">It's easy to verify the email forwarding settings on a mailbox!</span></span> <span data-ttu-id="c6697-106">다음 단계를 수행하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c6697-106">Just follow these steps.</span></span>
  
> <span data-ttu-id="c6697-107">사용자 사서함인 경우 사용자  활성 사용자로 이동하여 전달할 사서함을 가진 사용자를 \>  선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c6697-107">If this is a user mailbox, go to **Users** \> **Active users** and select the user whose mailbox you're forwarding.</span></span> <span data-ttu-id="c6697-108">메일 **탭에서** 전자 메일 전달 **관리를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="c6697-108">On the **Mail** tab, select **Manage email forwarding**.</span></span>

> <span data-ttu-id="c6697-109">공유 사서함인 경우 그룹  공유 사서함으로 이동하여 전달할 공유 \>  사서함을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c6697-109">If this is a shared mailbox, go to **Groups** \> **Shared mailboxes** and select the shared mailbox you're forwarding.</span></span> <span data-ttu-id="c6697-110">전자 **메일 전달에** 대한 편집을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c6697-110">Select **Edit** for email forwarding.</span></span>

<span data-ttu-id="c6697-111">자세한 내용은 [Microsoft 365에서](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)전자 메일 전달 구성을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c6697-111">For more information, see [Configure email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>
  
<span data-ttu-id="c6697-112">사용자가 자신의 사서함에서 전자 메일 전달을 설정할 수 있도록 사용자에게 지침을 보내기 위해 [Microsoft 365에서](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e)다른 전자 메일 계정으로 전자 메일 전달을 안내합니다.</span><span class="sxs-lookup"><span data-stu-id="c6697-112">To send instructions to your users so they can set up email forwarding on their own mailboxes, point them to [Forward email from Microsoft 365 to another email account](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e).</span></span> <span data-ttu-id="c6697-113">전자 메일 주소는 하나만 전달할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c6697-113">Please note that you can forward to only one email address.</span></span> <span data-ttu-id="c6697-114">사용자 그룹에 전달을 설정해야 하는 경우 메일 그룹(그룹 아래)을 만들고 해당 그룹에 사용자를 추가한 다음 해당 그룹에 전달을 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="c6697-114">If you need to set up forwarding to a group of people, create a distribution list (under **Groups**), add your users to it, and then configure forwarding to that group.</span></span>
  
<span data-ttu-id="c6697-115">직원이 퇴사하고 있나요?</span><span class="sxs-lookup"><span data-stu-id="c6697-115">Do you have an employee leaving?</span></span> <span data-ttu-id="c6697-116">권장 [단계는 Microsoft 365에서](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) 이전 직원 제거를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c6697-116">See [Remove a former employee from Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) for the recommended steps.</span></span>