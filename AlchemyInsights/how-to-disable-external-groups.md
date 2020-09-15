---
title: 외부 그룹을 사용 하지 않도록 설정 하는 방법
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704134"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="19c2a-102">외부 그룹을 사용 하지 않도록 설정 하는 방법</span><span class="sxs-lookup"><span data-stu-id="19c2a-102">How to disable External Groups</span></span>

<span data-ttu-id="19c2a-103">Yammer 외부 메시징은 회사 정보가 공유 되지 않도록 하는 자동 관리 제어 집합인 ETRs (Exchange 전송 규칙)를 적용 합니다.</span><span class="sxs-lookup"><span data-stu-id="19c2a-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="19c2a-104">사용자가 외부 그룹을 만들지 못하도록 제한 하려면 Exchange 전송 규칙 (ETR)을 구성한 다음 Exchange 전송 규칙을 사용 하 여 외부 메시지를 차단 하도록 Yammer를 구성 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="19c2a-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="19c2a-105">Exchange Online 관리 센터에서 규칙을 만들었으면 다음 단계에 따라 Yammer에서 ETR을 적용 하도록 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="19c2a-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="19c2a-106">확인 된 관리자로 Yammer에 로그온 하 고 **yammer 관리 센터**에서 C **콘텐츠 및 보안 \> 보안 설정으로 이동 합니다.**</span><span class="sxs-lookup"><span data-stu-id="19c2a-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="19c2a-107">**외부 메시징**에서 **Yammer에서 Exchange Online exchange 전송 규칙 (Etrs) 적용을 선택 합니다.**</span><span class="sxs-lookup"><span data-stu-id="19c2a-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="19c2a-108">**저장**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="19c2a-108">Choose **Save**.</span></span>

<span data-ttu-id="19c2a-109">자세한 내용은 [Yammer 네트워크에서 외부 메시징 사용 안 함을](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="19c2a-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  