---
title: OneDrive 충돌 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921013"
---
# <a name="troubleshoot-onedrive-crashes"></a>OneDrive 충돌 문제 해결

OneDrive가 반복적으로 충돌하는 경우 다음 문제 해결 단계를 시도해 보세요.

**레지스트리 키가 설정되어 있지 않은지 확인합니다.**

1. 레지스트리 편집기를 사용해 HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive로 이동합니다.
2. DisableFileSyncNGSC가 있고 1로 설정된 경우 키를 열고 값을 0으로 변경합니다.
3. 시작으로 이동하여 수동으로 OneDrive를 시작합니다. ![Windows 키 누르기](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)검색 상자에 OneDrive를 입력하십시오. 그 다음 OneDrive 데스크톱 앱을 클릭하십시오.

**OneDrive 초기화:**

참고:

- OneDrive를 다시 설정하면 모든 기존 동기화 연결이 끊어집니다(개인용 OneDrive가 설정된 경우 개인 OneDrive 포함).
- 컴퓨터에서 OneDrive를 다시 설정해도 파일이나 데이터가 손실되지는 않습니다.

**OneDrive를 초기화하려면:**

1. Windows 키 와 R을 눌러 실행 대화 상자를 여세요.
2. %localappdata%\Microsoft\OneDrive\onedrive.exe /reset을 입력하고 확인을 누릅니다. 명령 창이 잠깐 나타날 수 있습니다.
3. 시작으로 이동하여 수동으로 OneDrive를 시작합니다. ![Windows 키 누르기](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)검색 상자에 OneDrive를 입력하십시오. 그 다음 OneDrive 데스크톱 앱을 클릭하십시오.

참고:

- 다시 설정 전에 일부 폴더만 동기화하도록 선택한 경우 동기화가 완료되면 이 작업을 다시 해야 합니다. 자세한 내용은  [컴퓨터에 동기화할 OneDrive 폴더 선택](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) 을 읽어보세요.
- 개인용 OneDrive와 비즈니스용 OneDrive에 이 작업을 수행해야 합니다.