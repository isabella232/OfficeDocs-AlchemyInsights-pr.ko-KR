---
title: 요청 기반 파일 관리
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 10efdb5e1a90b3e279b8e1716e66a544d0ee34465245f5670930d8a9364a8cc3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53977447"
---
# <a name="configure-files-on-demand"></a>요청 기반 파일 관리 구성하기

OneDrive 요청 기반 파일 관리에는 [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (버전 1709 이상) 또는 Windows Server 2019 및 OneDrive 빌드 17.3.7064.1005 이상이 필요합니다.

OneDrive 요청 기반 파일 관리를 이용하면 파일을 다운로드하고 장치의 저장 공간을 사용하지 않아도 OneDrive의 모든 파일에 액세스할 수 있습니다.

PC에서 요청 기반 파일 관리를 구성하려면:

1. Windows 작업 표시줄 알림 영역에서 흰색 또는 파란색 **OneDrive** 구름 아이콘을 선택합니다. **도움말 및 설정** 톱니바퀴 아이콘 > **설정** 을 선택합니다.
2. **설정** 탭에서 **공간을 절약하고 사용할 때 파일 다운로드** 확인란을 선택합니다.  

레지스트리를 사용하여 요청 기반 파일 관리를 구성할 수도 있습니다.

이 설정을 사용하면 동기화 클라이언트를 설정한 새 사용자는 기본적으로 온라인 전용 파일을 다운로드합니다. 이 설정을 사용하지 않도록 설정하면 Windows 10 사용자는 이전 버전의 Windows 사용자와 동일한 동기화 동작을 진행하며, 요청 기반 파일을 설정할 수 없게 됩니다. 이 설정을 구성하지 않으면 사용자는 요청 기반 파일을 설정하거나 해제할 수 있습니다. 이 설정을 구성하지 않으면 사용자는 요청 기반 파일 관리를 켜거나 끌 수 있습니다.

이 정책을 사용하면 다음 레지스트리 키 값을 1로 설정합니다. 이 정책을 사용하지 않으면 다음 레지스트리 키 값을 0으로 설정합니다.

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

“설정”에서 요청 기반 파일 관리 옵션을 볼 수 없는 경우 서비스 "Windows 클라우드 파일 필터 드라이버" 시작 유형이 2 (AUTO_START)로 설정되어 있는지 확인합니다. 이 기능을 사용하면 다음 레지스트리 키 값을 2로 설정합니다.

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`