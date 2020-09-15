---
title: 2589 조직에서 보내는 전자 메일 메시지의 Winmail.dat 첨부 파일을 방지 하는 방법
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: f67c4146af419a590651c8e0673fd59fabd7eae7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47693741"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="d727a-102">조직의 전자 메일 메시지에 있는 Winmail.dat 첨부 파일을 차단 하는 방법</span><span class="sxs-lookup"><span data-stu-id="d727a-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="d727a-103">관리자는 다음 단계를 시도해 보세요.</span><span class="sxs-lookup"><span data-stu-id="d727a-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="d727a-104">[Exchange 관리 센터](https://outlook.office365.com/ecp/)를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="d727a-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="d727a-105">**메일 흐름**  >  **원격 도메인**으로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="d727a-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="d727a-106">**Default**라는 기본 원격 도메인을 선택 하 고 **편집**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="d727a-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="d727a-107">**서식 있는 텍스트 형식 사용** 섹션에서 **안 함을**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="d727a-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="d727a-108">자세한 내용은 [원격 도메인에 대 한 메시지 형식 지정](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format)을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="d727a-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
