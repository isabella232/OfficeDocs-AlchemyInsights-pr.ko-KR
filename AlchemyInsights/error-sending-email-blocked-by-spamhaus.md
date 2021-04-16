---
title: SpamHaus에서 차단된 전자 메일을 보내는 중 오류가 발생했습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813730"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="d84a6-102">전자 메일 보내기 오류: Spamhaus를 사용하여 클라이언트 호스트가 차단되었습니다.</span><span class="sxs-lookup"><span data-stu-id="d84a6-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="d84a6-103">메시지를 보낸 IP 주소는 [Spamhaus가](https://go.microsoft.com/fwlink/p/?linkid=123245)소유한 차단 목록에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d84a6-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="d84a6-104">Spamhaus가 차단하는 이유는 손상된 계정, 공용 IP 주소를 공유하는 손상된 컴퓨터 및 ISP(인터넷 서비스 공급자) 정책입니다.</span><span class="sxs-lookup"><span data-stu-id="d84a6-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="d84a6-105">가능한 해결 방법:</span><span class="sxs-lookup"><span data-stu-id="d84a6-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="d84a6-106">원본 전자 메일 서버를 제어하는 차단된 인바운드 메시지의 경우 원인을 파악하고 Spamhaus 웹 사이트에서 차단을 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d84a6-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="d84a6-107">원본 IP 주소가 다른 사람에게 속하는 차단된 인바운드 메시지의 경우 주소 소유자는 Spamhaus 웹 사이트에서 차단을 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d84a6-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="d84a6-108">IP 주소가 PBL(정책 차단 목록)에 있는 경우 소유자는 다른 고정 IP 주소를 할당하거나 PBL에서 주소를 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d84a6-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="d84a6-109">Microsoft에 연결된 도메인에서 보낸 차단된 아웃바운드 메시지의 경우 메시지가 제3자 서비스를 통해 라우팅되는 경우 이 오류를 수신할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d84a6-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="d84a6-110">WHOIS 검색 도구를 사용하여 차단된 IP 주소 소유자를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d84a6-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
