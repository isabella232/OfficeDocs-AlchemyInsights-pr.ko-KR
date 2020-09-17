---
title: SpamHaus에서 차단 된 전자 메일을 보내는 동안 오류 발생
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783809"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="2a2e1-102">전자 메일 보내기 오류: Spamhaus을 사용 하 여 클라이언트 호스트가 차단 됨</span><span class="sxs-lookup"><span data-stu-id="2a2e1-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="2a2e1-103">메시지를 보낸 IP 주소가 [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)에서 소유한 차단 목록에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="2a2e1-104">Spamhaus에 의해 차단 되는 이유에는 손상 된 계정, 공용 IP 주소를 공유 하는 손상 된 컴퓨터 및 ISP (인터넷 서비스 공급자) 정책이 포함 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="2a2e1-105">가능한 수정은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="2a2e1-106">원본 전자 메일 서버를 제어 하는 차단 된 인바운드 메시지의 경우 원인을 확인 하 고 Spamhaus 웹 사이트에서 해당 블록을 제거 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="2a2e1-107">원본 IP 주소가 다른 사람에 게 속하는 차단 된 인바운드 메시지의 경우 주소 소유자가 Spamhaus 웹 사이트에서 해당 블록을 제거 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="2a2e1-108">IP 주소가 정책 차단 목록 (PBL)에 있는 경우 소유자는 다른 고정 IP 주소를 할당 하거나 PBL에서 주소를 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="2a2e1-109">Microsoft에 연결 된 도메인에서 차단 된 아웃 바운드 메시지의 경우 메시지가 타사 서비스를 통해 라우팅되는 경우이 오류를 수신할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="2a2e1-110">WHOIS 조회 도구를 사용 하 여 차단 된 IP 주소 소유자를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2a2e1-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
