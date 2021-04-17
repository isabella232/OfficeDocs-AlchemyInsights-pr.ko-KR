---
title: 전자 메일 catch 모두 만들기
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816206"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="2aecf-102">전자 메일 catch 모두 만들기</span><span class="sxs-lookup"><span data-stu-id="2aecf-102">Create an email catch all</span></span>

<span data-ttu-id="2aecf-103">catch를 모두 사용하는 것은 강력히 금지됩니다.</span><span class="sxs-lookup"><span data-stu-id="2aecf-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="2aecf-104">보낸 사람이 조치를 취할 수 있도록 보낸 사람이 메시지를 주소로 배달할 수 없다고 알려주는 반송을 보낸 사람에 제공하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="2aecf-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="2aecf-105">모니터링되는 사서함이 이전의 유효한 전자 메일 주소만 catch하는 것으로 제한할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2aecf-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="2aecf-106">모든 catch 모든 사서함은 스팸을 상당 부분을 받으며 면밀하게 모니터링하지 않는 경우 결국 채울 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2aecf-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="2aecf-107">수신 제한이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2aecf-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="2aecf-108">계속하기로 결정한 경우 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="2aecf-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="2aecf-109">"모든 받는 사람 유형"& 메일 그룹 만들기</span><span class="sxs-lookup"><span data-stu-id="2aecf-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="2aecf-110">예를 들어 전자 메일을 catch하기 위한 전용 사서함을 catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="2aecf-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="2aecf-111">특정 도메인의 경우 DomainType을 "InternalRelay"로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="2aecf-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="2aecf-112">나중에 catch를 모두 제거하는 경우 도메인을 다시 Authoritative로 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2aecf-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="2aecf-113">다음과 같이 메일 흐름 전송 규칙을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2aecf-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="2aecf-114">보낸 사람이 "조직 외부"인 경우</span><span class="sxs-lookup"><span data-stu-id="2aecf-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="2aecf-115">메시지를 메시지로 Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="2aecf-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="2aecf-116">받는 사람이 allusers@domain.com 구성원인 경우를 제외하고(메일 그룹에 모든 구성원 포함)</span><span class="sxs-lookup"><span data-stu-id="2aecf-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="2aecf-117">새 사서함이 동적 메일 그룹에 추가되는지 확인</span><span class="sxs-lookup"><span data-stu-id="2aecf-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
