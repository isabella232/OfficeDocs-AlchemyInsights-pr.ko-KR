---
title: 여러 개체의 전자 메일 주소가 ID와 동일합니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431536"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="ccb17-102">여러 개체의 전자 메일 주소가 ID와 동일합니다.</span><span class="sxs-lookup"><span data-stu-id="ccb17-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="ccb17-103">**여러 개체**</span><span class="sxs-lookup"><span data-stu-id="ccb17-103">**Multiple objects**</span></span>

<span data-ttu-id="ccb17-104">이 오류가 발생하는 일반적인 이유 중 하나는 전자 메일 주소가 ID와 동일한 여러 개체가 존재하여 Outlook Web Access 요청을 올바르게 라우팅할 수 없기 때문입니다.</span><span class="sxs-lookup"><span data-stu-id="ccb17-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="ccb17-105">이와 같은 개체를 찾으려면 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="ccb17-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="ccb17-106">· Get-Recipient <email address></span><span class="sxs-lookup"><span data-stu-id="ccb17-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="ccb17-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="ccb17-107">· Get-User <email address></span></span>

<span data-ttu-id="ccb17-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="ccb17-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="ccb17-109">· Get-Contact <email address></span><span class="sxs-lookup"><span data-stu-id="ccb17-109">· Get-Contact <email address></span></span>

<span data-ttu-id="ccb17-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="ccb17-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="ccb17-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="ccb17-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="ccb17-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="ccb17-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="ccb17-113">이 문제를 해결하려면 동일한 전자 메일 ID가 있는 여러 개체를 제거하고 특정 전자 메일 ID가 포함된 단일 개체가 있고 해당하는 받는 사람 형식이 UserMailbox인지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ccb17-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="ccb17-114">**동일한 주소가 비즈니스 및 소비자 사서함에 사용됩니다.**</span><span class="sxs-lookup"><span data-stu-id="ccb17-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="ccb17-115">또 다른 원인은 동일한 주소를 비즈니스 및 소비자 사서함에 사용하는 경우입니다.</span><span class="sxs-lookup"><span data-stu-id="ccb17-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="ccb17-116">이 경우, 카페에서 이 시나리오를 지원할 때까지는 사용자가 기본 소비자 별칭을 변경해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ccb17-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="ccb17-117">이는 개입 없이는 사라지지 않는 영구적인 오류입니다.</span><span class="sxs-lookup"><span data-stu-id="ccb17-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="ccb17-118">자세한 내용은 [Microsoft 계정의 전자 메일 주소 또는 전화 번호 변경](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ccb17-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>