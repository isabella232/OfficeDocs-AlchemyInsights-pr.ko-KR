---
title: Microsoft 365 앱에 로그인하는 문제
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
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709112"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="fd843-102">Microsoft 365 앱 수정 "컴퓨터의 신뢰할 수 있는 플랫폼 모듈이 제대로 작동하지 않습니다." 메시지</span><span class="sxs-lookup"><span data-stu-id="fd843-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="fd843-103">이 오류를 해결하려면 다음 단계를 수행하십시오.</span><span class="sxs-lookup"><span data-stu-id="fd843-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="fd843-104">Windows 및 [Office용 최신 업데이트를](https://support.microsoft.com/help/4027667/windows-10-update) [설치합니다.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="fd843-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="fd843-105">Windows [자격 증명 관리자를](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) 사용하여 Office 자격 증명 지우기</span><span class="sxs-lookup"><span data-stu-id="fd843-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="fd843-106">**참고:** Office 2016의 레지스트리 경로가 16.0으로 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="fd843-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="fd843-107">(예: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="fd843-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="fd843-108">사용자 [복구 프로세스를 시도하여](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) TPM(신뢰할 수 있는 플랫폼 모듈) 오류를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="fd843-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="fd843-109">다음 단계를 사용하여 EnableADAL = 0을 설정하십시오.</span><span class="sxs-lookup"><span data-stu-id="fd843-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="fd843-110">Windows 시작 단추를 마우스 오른쪽 단추로 클릭하고 **실행을** 선택하고 **regedit를** 입력한 다음 확인 을 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="fd843-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="fd843-111">레지스트리 **편집기에서** 장치를 변경할 수 있도록 허용하려면 예를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="fd843-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="fd843-112">레지스트리 편집기에서 설정값이 **0인** **EnableADAL의** DWORD 값을 HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="fd843-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="fd843-113">자세한 내용은 [Windows 10의 Office 2016 빌드 16.0.7967로](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)업데이트한 후 로그인 시 연결 문제를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="fd843-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>