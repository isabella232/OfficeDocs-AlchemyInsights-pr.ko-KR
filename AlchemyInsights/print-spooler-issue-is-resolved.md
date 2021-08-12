---
title: 인쇄 스풀러 문제 해결됨
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911344"
---
# <a name="print-spooler-issue-is-resolved"></a>인쇄 스풀러 문제 해결됨

장치를 Windows 10 **OS 빌드 19041.329** 로 업데이트한 경우 특정 프린터에서 인쇄가 되지 않는 문제가 발생할 수 있습니다. 인쇄를 하려고 할 때 인쇄 스풀러가 오류가 일으키거나 예기치 않게 종료될 수 있으며, 영향을 받는 프린터에서 출력이 전송되지 않을 수 있습니다. 이 문제는 OS 빌드 **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)에서 해결했습니다.  

**진행 중인 조사**

일부 장치의 LSASS(Local Security Authority Subsystem Service) 파일(**Isass**)에서 ‘중요 시스템 프로세스인 C:\WINDOWS\system32\Isass.exe에 오류가 발생했으며 상태 코드는 c0000008입니다. 지금 컴퓨터를 재시작해야 합니다’라는 오류 메시지가 포함된 오류가 발생할 수 있습니다.  **Microsoft는 문제 해결을 위해 노력 중이며 예정된 릴리스에서 업데이트를 제공할 예정입니다.**

자세한 내용은 [Windows 10 버전 2004에서 알려진 문제](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)를 확인하세요.