---
title: Microsoft 365 앱 수정 죄송합니다. 임시 서버 문제 메시지가 있습니다.
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835277"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="c72fe-102">Microsoft 365 앱 수정 "죄송합니다. 일시적인 서버 문제가 있습니다" 메시지 수정</span><span class="sxs-lookup"><span data-stu-id="c72fe-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="c72fe-103">이 메시지를 받으면 다음을 시도해 보아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c72fe-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="c72fe-104">방화벽, 바이러스 백신 소프트웨어 및 프록시 설정을 확인하여 Microsoft 365 앱에 대한 인터넷 액세스를 차단하지 않는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c72fe-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="c72fe-105">URL [및 IP 주소 범위를 참조하세요.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="c72fe-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="c72fe-106">시작   >  **실행으로 이동한** 다음 **services.msc 를 입력합니다.**</span><span class="sxs-lookup"><span data-stu-id="c72fe-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="c72fe-107">다음 서비스가 모두 실행 중인지 확인</span><span class="sxs-lookup"><span data-stu-id="c72fe-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="c72fe-108">네트워크 연결 장치 자동 설정</span><span class="sxs-lookup"><span data-stu-id="c72fe-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="c72fe-109">네트워크 목록 서비스</span><span class="sxs-lookup"><span data-stu-id="c72fe-109">Network List Service</span></span>
    - <span data-ttu-id="c72fe-110">네트워크 위치 인식</span><span class="sxs-lookup"><span data-stu-id="c72fe-110">Network Location Awareness</span></span>
    - <span data-ttu-id="c72fe-111">Windows 이벤트 로그</span><span class="sxs-lookup"><span data-stu-id="c72fe-111">Windows Event Log</span></span>

<span data-ttu-id="c72fe-112">이러한 서비스 중 하나에서 실행되고 있지 않은 경우 시작해 보아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c72fe-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="c72fe-113">서비스를 시작하는 데 문제가 있는 경우 상승된 사용 권한으로 명령 프롬프트를 열고 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="c72fe-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="c72fe-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="c72fe-114">**sfc /scannow**</span></span>

<span data-ttu-id="c72fe-115">이 명령이 완료되면 컴퓨터를 다시 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="c72fe-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="c72fe-116">자세한 내용은 ["죄송합니다. 계정에 연결할 수 없습니다. 나중에 다시 시도하세요" 오류를 활성화하면 오류가 발생합니다.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="c72fe-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>