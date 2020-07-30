---
title: TeamViewer를 사용하여 Intune 장치 원격 관리
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505212"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>TeamViewer를 사용하여 Intune 장치 원격 관리

Intune에서 관리하는 장치는 [TeamViewer](https://www.teamviewer.com/)를 사용하여 원격으로 관리할 수 있습니다.

TeamViewer를 사용하여 Intune을 관리하려면 다음 단계를 사용합니다. 

먼저 TeamViewer에서 자격 증명을 가져와서 시작하여 Intune에서 TeamViewer 커넥터를 설정합니다. 이렇게 하면 관리자가 TeamViewer 커넥터 UI의 장치 아래에 자격 증명을 입력하고, 한 번의 작업으로 Intune과 TeamViewer 서비스 간에 연결을 설정할 수 있습니다.

**1부: 원격 장치를 사용하여 세션 시작**

1. **모든 장치**에서 원격 세션을 시작하려는 장치를 선택합니다.
2. **...추가**에서 **새 원격 지원 세션**을 선택합니다.
3. 원격 세션 설정을 승인하려면 **예**를 선택합니다.
    TeamViewer 서비스에서 "새 원격 세션 시작" 요청을 승인하고 나면, 장치의 개요(또는 필수) 세부 정보 창 아래에서 **원격 지원 시작** 옵션이 표시됩니다. 창을 확장하고 원격 지원 상태를 표시하려면 **더 보기**를 참조하세요.
4. **원격 세션 시작**을 선택하여 관리자 측에서 세션을 시작합니다.
5. TeamViewer 바이너리(Windows)를 다운로드하도록 선택하고 **실행**을 선택합니다.<br/>
    **참고** TeamViewer 웹 사이트에 열린 모든 웹 브라우저 페이지를 무시할 수 있습니다.

6. TeamViewer 앱에 대한 요청을 승인하여 장치(Windows만 해당)에 대해 변경할 수 있습니다.
7. TeamViewer 앱이 시작되며 원격 장치에 대한 연결을 인증하기 위한 세션 코드를 포함합니다.

**2부: 원격 세션을 대상으로 하는 장치에서**

1. Intune 회사 포털을 엽니다.
2. "IT 관리자가 원격 지원 세션에서 이 장치의 제어권을 요청하고 있습니다."라는 알림 플래그를 찾고 해당 알림을 선택합니다.
3. TeamViewer 응용 프로그램을 다운로드하도록 선택하거나 App Store에서 TeamViewer 앱 다운로드를 승인하고 **실행**을 선택합니다.
    **참고** TeamViewer 웹 사이트에 열린 모든 웹 브라우저 페이지를 무시할 수 있습니다.

4. TeamViewer 앱에 대한 요청을 승인하여 장치(Windows만 해당)에 대해 변경할 수 있습니다.
5. TeamViewer 앱이 시작되며 원격 장치에 대한 연결을 인증하기 위한 세션 코드를 포함합니다.
6. 세션을 시작할 것인지 묻는 팝업이 표시됩니다.

**참고** TeamViewer 서비스에서 생성되는 세션 코드는 일회용입니다. 연결이 끊긴 경우 다음을 수행해야 합니다.

1. 원격 장치 및 관리자 워크스테이션에서 TeamViewer 앱의 인스턴스를 닫습니다.
2. 원격 장치에서 회사 포털을 닫습니다.
3. 관리자 포털에서 "새 원격 지원 세션"을 시작합니다.
4. 새 알림을 받으려면 원격 장치에서 회사 포털을 다시 엽니다.
5. 이전과 마찬가지로, 원격 장치와 관리자 워크스테이션에서 TeamViewer 앱을 다운로드하고 엽니다.