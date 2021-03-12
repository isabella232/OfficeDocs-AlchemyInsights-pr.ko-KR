---
title: 특정 Office 365 전자 메일 메시지 자동 암호화
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736826"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="9f388-102">특정 Office 365 전자 메일 메시지 자동 암호화</span><span class="sxs-lookup"><span data-stu-id="9f388-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="9f388-103">사용자가 특정 외부 사람 또는 조직에 보내는 메시지를 자동으로 암호화할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9f388-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="9f388-104">이 작업을 수행 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="9f388-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="9f388-105">Exchange 관리 [센터에서](https://outlook.office365.com/ecp/)메일 흐름 > **를 선택하세요.**</span><span class="sxs-lookup"><span data-stu-id="9f388-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="9f388-106">새로 **추가(+) 아이콘을** 클릭한 다음 메시지에 **Office 365** 메시지 암호화 및 권한 보호 적용을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="9f388-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="9f388-107">이름 **에** 규칙의 이름(예: 에 전송된 메시지 *암호화)을* DrToniRamos@gmail.com.</span><span class="sxs-lookup"><span data-stu-id="9f388-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="9f388-108">다음의 경우 이 **규칙** 적용에서 받는 **사람 > 를 선택 합니다.**</span><span class="sxs-lookup"><span data-stu-id="9f388-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="9f388-109">구성원 **선택 창에서** 암호화 규칙을 적용할 사람의 이름을 선택하고 추가를 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="9f388-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="9f388-110">사용자 추가를 완료하면 확인 을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="9f388-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="9f388-111">다음 작업을 **진행하십시오. 필드 옆에** 있는 하나 **선택을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="9f388-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="9f388-112">**RMS 템플릿** 드롭다운 메뉴에서 **암호화를** 선택하고 확인 을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="9f388-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="9f388-113">(이 옵션이 없는 경우 요금제에 자동 암호화가 포함되어하지 않는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="9f388-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="9f388-114">하지만 추가할 수 있습니다!)</span><span class="sxs-lookup"><span data-stu-id="9f388-114">But you can add it!)</span></span>
9. <span data-ttu-id="9f388-115">선택 사항(이 시점에서 만들 수 있는 선택 사항 목록에서 선택 사항 중 다수는 단순성을 위한 기본 설정으로 남을 수 있습니다)을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="9f388-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="9f388-116">**저장** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="9f388-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9f388-117">언제든지 돌아와서 나중에 이 규칙을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9f388-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="9f388-118">암호화 규칙을 만드는 데 대한 자세한 내용은 [Office 365에서](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)전자 메일 메시지를 암호화하는 메일 흐름 규칙 정의를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9f388-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

