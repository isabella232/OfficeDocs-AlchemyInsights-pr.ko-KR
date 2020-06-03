---
title: 웹용 Outlook의 S/MIME
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511514"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="96271-102">Outlook에서 전자 메일 메시지 암호화</span><span class="sxs-lookup"><span data-stu-id="96271-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="96271-103">Microsoft 365 메시지 암호화는 Azure Information Protection의 일부인 Azure RMS (Microsoft Azure Rights Management)를 기반으로 합니다.</span><span class="sxs-lookup"><span data-stu-id="96271-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="96271-104">Azure 권한 관리 또는 Azure Information Protection이 구독에 포함 되어 있는 경우에는 권한 관리 서비스를 **수동으로 사용 하거나 활성화 하기 위해 작업을 수행할 필요가 없습니다** .</span><span class="sxs-lookup"><span data-stu-id="96271-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="96271-105">고객 의견에 따라 더 이상 Exchange 메일 흐름 규칙을 사용 하 여 테 넌 트에 특정 유형의 중요 한 정보를 포함 하는 아웃 바운드 전자 메일을 기본적으로 자동 암호화 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="96271-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="96271-106">대신이 yourselves를 수행 하는 방법에 대 한 자세한 지침을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="96271-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="96271-107">중요 한 정보를 암호화 하는 전송 규칙을 만드는 방법에 대 한 자세한 내용은 [이 문서](https://aka.ms/OmeEtr)를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="96271-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="96271-108">웹용 Outlook (이전에는 **owa**)을 사용 하는 경우 전자 메일 메시지를 작성할 때 Owa에서 **보호** 를 클릭 하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="96271-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="96271-109">이렇게 하면 "전달 금지" 권한이 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="96271-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="96271-110">**사용 권한 변경을** 클릭 하 고 **암호화** 를 선택 하 여 메시지만 암호화 합니다.</span><span class="sxs-lookup"><span data-stu-id="96271-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="96271-111">**Outlook 클라이언트**를 사용 하는 경우: outlook 2013 또는 2016 또는 Mac 용 outlook 2016에서 암호화 된 메시지를 보내려면 **옵션**  >  **사용 권한을**선택 하 고 필요한 보호 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="96271-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="96271-112">특정 받는 사람이 나 외부 파트너 조직에 보낸 **모든 전자 메일을 자동으로 암호화** 하려면 Exchange 관리 센터에서 메일 흐름 전송 규칙을 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="96271-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="96271-113">자세한 지침은 [이 지원 문서](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)에 나와 있습니다.</span><span class="sxs-lookup"><span data-stu-id="96271-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

