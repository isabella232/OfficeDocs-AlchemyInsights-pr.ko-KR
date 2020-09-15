---
title: Microsoft 365 앱에 로그인 하는 문제
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695293"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="49ba3-102">Microsoft 365 앱의 빈 로그인 화면</span><span class="sxs-lookup"><span data-stu-id="49ba3-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="49ba3-103">이 문제를 해결 하려면 다음을 시도 합니다.</span><span class="sxs-lookup"><span data-stu-id="49ba3-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="49ba3-104">[Windows](https://support.microsoft.com/help/4027667/windows-10-update) 및 [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)용 최신 업데이트를 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="49ba3-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="49ba3-105">Internet explorer 옵션 다시 설정: **도구**  >  **인터넷 옵션**  >  **고급**  >  **재설정 internet explorer 설정** (사용자 지정 설정이 손실 됨)을 확인 한 후 다시 Office에 로그인을 시도 합니다.</span><span class="sxs-lookup"><span data-stu-id="49ba3-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="49ba3-106">Windows Defender Application Guard (WDAG) 또는 이와 유사한 모든 방화벽 또는 바이러스 백신 프로그램을 사용 하지 않도록 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="49ba3-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="49ba3-107">제어판에서 **프로그램**으로 이동한 다음 **Windows 기능 사용 또는 해제**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="49ba3-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="49ba3-108">Windows Defender Application Guard를 사용 하도록 설정 된 경우 사용 하지 않도록 설정 해 봅니다.</span><span class="sxs-lookup"><span data-stu-id="49ba3-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="49ba3-109">**참고:** 컴퓨터를 다시 시작 해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="49ba3-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="49ba3-110">BrokerPlugin [AAD WAM 플러그](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) 인이 모든 응용 프로그램 또는 방화벽/바이러스 백신 프로그램에 의해 차단 되지 않는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="49ba3-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="49ba3-111">Windows Credential Manager를 사용 하 여 [Office 자격 증명을 지웁니다](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .</span><span class="sxs-lookup"><span data-stu-id="49ba3-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="49ba3-112">**참고:** Office 2016의 레지스트리 경로가 16.0로 변경 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="49ba3-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="49ba3-113">(예: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="49ba3-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="49ba3-114">자세한 내용은 [Windows 10의 업데이트 후 Office 2016 빌드 16.0.7967에 로그인 후 연결 문제](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="49ba3-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>