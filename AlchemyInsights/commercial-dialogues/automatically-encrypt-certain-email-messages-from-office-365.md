---
title: Office 365에서 특정 전자 메일 메시지 자동 암호화
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736829"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="ebc13-102">Office 365에서 특정 전자 메일 메시지 자동 암호화</span><span class="sxs-lookup"><span data-stu-id="ebc13-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="ebc13-103">Exchange 관리 [센터에서](https://outlook.office365.com/ecp/)메일 흐름 > **를 선택하세요.**</span><span class="sxs-lookup"><span data-stu-id="ebc13-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="ebc13-104">새로 **추가(+) 아이콘을** 클릭한 다음 메시지에 **Office 365** 메시지 암호화 및 권한 보호 적용을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ebc13-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="ebc13-105">이름에 모든 메시지 암호화와 같은 규칙의 *이름을 입력합니다.* </span><span class="sxs-lookup"><span data-stu-id="ebc13-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="ebc13-106">다음의 경우 이 **규칙 적용에서**[모든 메시지에 **적용] 을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="ebc13-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="ebc13-107">다음 작업을 **진행하십시오. 필드 옆에** 있는 하나 **선택을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="ebc13-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="ebc13-108">**RMS 템플릿** 드롭다운 메뉴에서 **암호화를** 선택하고 확인 을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="ebc13-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="ebc13-109">(이 옵션이 없는 경우 요금제에 자동 암호화가 포함되어하지 않는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="ebc13-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="ebc13-110">하지만 추가할 수 있습니다!)</span><span class="sxs-lookup"><span data-stu-id="ebc13-110">But you can add it!)</span></span>
7. <span data-ttu-id="ebc13-111">심각도 **수준으로** 이 규칙 감사 확인란을 선택한 다음 원하는 수준을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ebc13-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="ebc13-112">회사에서 암호화된 모든 전자 메일을 보낼 계약상 의무가 있는 경우 수준을 높음으로 설정하는 것이 **좋습니다.**</span><span class="sxs-lookup"><span data-stu-id="ebc13-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="ebc13-113">이 **규칙에 대한 모델 선택에서** 적용을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="ebc13-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="ebc13-114">선택 사항(이 시점에서 만들 수 있는 선택 사항 목록에서 선택 사항 중 다수는 단순성을 위한 기본 설정으로 남을 수 있습니다)을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ebc13-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="ebc13-115">**저장** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ebc13-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ebc13-116">언제든지 돌아와서 나중에 이 규칙을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ebc13-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="ebc13-117">암호화 규칙을 만드는 데 대한 자세한 내용은 [Define mail flow rules to encrypt email messages in Office 365를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="ebc13-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

