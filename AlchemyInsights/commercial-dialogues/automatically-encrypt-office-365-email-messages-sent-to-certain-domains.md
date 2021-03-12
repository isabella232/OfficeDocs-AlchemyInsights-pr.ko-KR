---
title: 특정 도메인으로 전송되는 Office 365 전자 메일 메시지 자동 암호화
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736781"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="def56-102">특정 도메인으로 전송되는 Office 365 전자 메일 메시지 자동 암호화</span><span class="sxs-lookup"><span data-stu-id="def56-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="def56-103">Exchange 관리 [센터에서](https://outlook.office365.com/ecp/)메일 흐름 > **를 선택하세요.**</span><span class="sxs-lookup"><span data-stu-id="def56-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="def56-104">새로 **추가(+) 아이콘을** 클릭한 다음 메시지에 **Office 365** 메시지 암호화 및 권한 보호 적용을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="def56-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="def56-105">이름 **에** 규칙의 이름(예: 에 전송된 메시지 *암호화)을* contoso.com.</span><span class="sxs-lookup"><span data-stu-id="def56-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="def56-106">다음의 경우 이 **규칙 적용에서** 받는 사람 > **를 선택 합니다.**</span><span class="sxs-lookup"><span data-stu-id="def56-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="def56-107">도메인 이름(예: 을(를) **contoso.com.**</span><span class="sxs-lookup"><span data-stu-id="def56-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="def56-108">**추가(+) 아이콘을** 클릭한 다음 확인을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="def56-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="def56-109">다음 작업을 **진행하십시오. 필드 옆에** 있는 하나 **선택을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="def56-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="def56-110">**RMS 템플릿** 드롭다운 메뉴에서 **암호화를** 선택하고 확인 을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="def56-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="def56-111">(이 옵션이 없는 경우 요금제에 자동 암호화가 포함되어하지 않는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="def56-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="def56-112">하지만 추가할 수 있습니다!)</span><span class="sxs-lookup"><span data-stu-id="def56-112">But you can add it!)</span></span>
9. <span data-ttu-id="def56-113">선택 사항(이 시점에서 만들 수 있는 선택 사항 목록에서 선택 사항 중 다수는 단순성을 위한 기본 설정으로 남을 수 있습니다)을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="def56-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="def56-114">**저장** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="def56-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="def56-115">언제든지 돌아와서 나중에 이 규칙을 편집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="def56-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="def56-116">암호화 규칙을 만드는 데 대한 자세한 내용은 [Define mail flow rules to encrypt email messages in Office 365를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="def56-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>