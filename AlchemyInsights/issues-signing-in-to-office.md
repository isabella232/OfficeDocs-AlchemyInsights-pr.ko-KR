---
title: Microsoft 365 앱에 로그인하는 문제
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
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833045"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="85fcc-102">Microsoft 365 앱의 빈 로그인 화면</span><span class="sxs-lookup"><span data-stu-id="85fcc-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="85fcc-103">이 문제를 해결하려는 경우 다음을 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="85fcc-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="85fcc-104">Windows 및 [Office용 최신 업데이트를](https://support.microsoft.com/help/4027667/windows-10-update) [설치합니다.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="85fcc-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="85fcc-105">사용자 Internet Explorer 다시 설정: 도구 인터넷 옵션 고급 초기화 Internet Explorer 설정으로 이동한 다음(사용자 지정 설정이 손실) Office에 다시 로그인해  >    >    >   보십시오.</span><span class="sxs-lookup"><span data-stu-id="85fcc-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="85fcc-106">WDAG(Windows Defender Application Guard) 또는 유사한 방화벽 또는 바이러스 백신 프로그램을 사용하지 않도록 설정:</span><span class="sxs-lookup"><span data-stu-id="85fcc-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="85fcc-107">제어판에서 프로그램으로 이동한 다음 Windows 기능 켜기 **또는 끄기 를 선택 합니다.**</span><span class="sxs-lookup"><span data-stu-id="85fcc-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="85fcc-108">Application Guard를 Windows Defender 경우 이 기능을 사용 안 하게 합니다.</span><span class="sxs-lookup"><span data-stu-id="85fcc-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="85fcc-109">**참고:** 컴퓨터를 다시 시작해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85fcc-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="85fcc-110">Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) 플러그 인이 응용 프로그램 또는 방화벽/바이러스 백신 프로그램에 의해 차단되지 않는지 확인</span><span class="sxs-lookup"><span data-stu-id="85fcc-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="85fcc-111">Windows [자격 증명 관리자를](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) 사용하여 Office 자격 증명 지우기</span><span class="sxs-lookup"><span data-stu-id="85fcc-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="85fcc-112">**참고:** Office 2016의 레지스트리 경로가 16.0으로 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="85fcc-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="85fcc-113">(예: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="85fcc-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="85fcc-114">자세한 내용은 [Windows 10의 Office 2016 빌드 16.0.7967로](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)업데이트한 후 로그인 시 연결 문제를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="85fcc-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>