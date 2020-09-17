---
title: Teams 클라이언트의 작동이 중지되나요?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 39310233eae83ceb18c6ff82451ae747f3c50048
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691113"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="20f1e-102">Teams 클라이언트의 작동이 중지되나요?</span><span class="sxs-lookup"><span data-stu-id="20f1e-102">Teams client crashing?</span></span>

<span data-ttu-id="20f1e-103">Teams 클라이언트의 작동이 중단되면 다음을 시도해 보세요.</span><span class="sxs-lookup"><span data-stu-id="20f1e-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="20f1e-104">Teams 데스크톱 앱을 사용하는 경우 [앱이 완전히 업데이트되었는지 확인합니다](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="20f1e-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="20f1e-105">모든 [Microsoft 365 URL 및 주소 범위](https://docs.microsoft.com/microsoftteams/connectivity-issues)에 액세스할 수 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="20f1e-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="20f1e-106">테넌트 관리자 계정으로 로그인하고 [서비스 상태 대시보드](https://docs.microsoft.com/office365/enterprise/view-service-health)를 확인하여 작동 중단 또는 서비스 저하가 없는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="20f1e-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="20f1e-107">Teams 애플리케이션 제거 및 다시 설치(링크)</span><span class="sxs-lookup"><span data-stu-id="20f1e-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="20f1e-108">컴퓨터에서 %appdata%\Microsoft\teams\ folder로 이동하고 디렉터리의 모든 파일을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="20f1e-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="20f1e-109">[Teams 앱을 다운로드 및 설치](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)하고 가능한 경우, 관리자로 Teams를 설치합니다(Teams 설치 관리자를 오른쪽 마우스로 클릭하고 가능한 경우 “관리자로 실행” 선택).</span><span class="sxs-lookup"><span data-stu-id="20f1e-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="20f1e-110">Teams 클라이언트가 계속 충돌하는 경우, 문제를 재현할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="20f1e-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="20f1e-111">그럴 경우, 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="20f1e-111">If so:</span></span>

1. <span data-ttu-id="20f1e-112">단계 레코더를 사용하여 단계를 캡처할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="20f1e-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="20f1e-113">불필요하거나 중요한 응용 프로그램을 모두 종료합니다.</span><span class="sxs-lookup"><span data-stu-id="20f1e-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="20f1e-114">단계 레코더를 시작하고 영향을 받은 사용자 계정으로 로그인하여 문제를 재현해 보세요.</span><span class="sxs-lookup"><span data-stu-id="20f1e-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="20f1e-115">[기록한 재현 단계를 캡처하는 팀 로그를 수집합니다](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="20f1e-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="20f1e-116">**참고**: 영향을 받은 사용자의 로그인 주소를 캡처해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="20f1e-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="20f1e-117">덤프 및/또는 오류 버킷 정보를 수집합니다(Windows).</span><span class="sxs-lookup"><span data-stu-id="20f1e-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="20f1e-118">충돌이 발생하는 컴퓨터에서 Windows Powershell을 실행하고 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="20f1e-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="20f1e-119">고객 지원 서비스 케이스에 파일을 첨부합니다.</span><span class="sxs-lookup"><span data-stu-id="20f1e-119">Attach the file to your support case.</span></span>
