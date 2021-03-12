---
title: TLS 1.0 및 TLS 1.1 비활성화로 인하여 Office 365로 전자 메일을 보내고 받을 수 없습니다.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726938"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="2e027-102">TLS 1.0 및 TLS 1.1 비활성화로 인하여 Office 365로 전자 메일을 보내고 받을 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="2e027-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="2e027-103">MC229914 메시지 센터에서 확인한 결과, TLS 1.0 및 TLS 1.1 사용 중단이 Exchange Online 메일 흐름 끝점에 대해 강요하기 시작했습니다.</span><span class="sxs-lookup"><span data-stu-id="2e027-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="2e027-104">곧 Office 365에서 외부 원본의 TLS 1.0 및 TLS 1.1 전자 메일 연결을 더 이상 수락하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2e027-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="2e027-105">또한 Exchange Online에서는 TLS 1.0 또는 1.1을 사용하여 아웃바운드 전자 메일을 보내지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2e027-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="2e027-106">TLS 1.0 또는 1.1 비활성화로 문제가 발생하는 경우 다음 오류 중 하나를 경험할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2e027-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="2e027-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span><span class="sxs-lookup"><span data-stu-id="2e027-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="2e027-108">관리자 365- '421 4.4.2 SocketError로 인해 연결이 끊어졌다'에게 전자 메일을 보내는 On-Premises 서버의 큐 뷰어에서 오류가 발생했습니다.</span><span class="sxs-lookup"><span data-stu-id="2e027-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="2e027-109">송신 커넥터 [프로토콜 로그에서](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) 오류가 발생하여 Office 365로 전자 메일을 보내는 서버의 프로토콜 로그에서 오류가 발생했습니다. 오류 SocketError로 TLS 협상에 실패했습니다.</span><span class="sxs-lookup"><span data-stu-id="2e027-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="2e027-110">송신 또는 수신 커넥터 프로토콜 로그 오류 - '451 5.7.3 STARTTLS 명령을 먼저 실행해야 합니다'</span><span class="sxs-lookup"><span data-stu-id="2e027-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="2e027-111">위의 오류가 발생하는 경우 다음 레지스트리 키를 확인하여 전자 메일을 보내거나 받는 서버에 TLS 1.2가 사용하도록 설정되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2e027-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="2e027-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:000000001**</span><span class="sxs-lookup"><span data-stu-id="2e027-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="2e027-113">위의 레지스트리 키를 변경하여 TLS 1.2를 사용하도록 설정한 경우 서버를 다시 시작하여 변경 내용을 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="2e027-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="2e027-114">또한 최신 Windows 및 Exchange 업데이트가 설치되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2e027-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="2e027-115">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2e027-115">For more information, see:</span></span>

- [<span data-ttu-id="2e027-116">Exchange Server TLS 지침, 1부: TLS 1.2 준비 - Microsoft 기술 커뮤니티</span><span class="sxs-lookup"><span data-stu-id="2e027-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="2e027-117">Exchange Server TLS 지침 2부: TLS 1.2를 사용하도록 설정하고 사용하지 않는 클라이언트 식별 - Microsoft 기술 커뮤니티</span><span class="sxs-lookup"><span data-stu-id="2e027-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="2e027-118">TLS 버전이 Exchange Online과 합의할 수 없는 경우 전자 메일 시나리오 이해 - Microsoft 기술 커뮤니티</span><span class="sxs-lookup"><span data-stu-id="2e027-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
