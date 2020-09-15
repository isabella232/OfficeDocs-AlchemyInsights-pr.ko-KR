---
title: 오류:이 컴퓨터의 규칙이 일치 하지 않습니다.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690969"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>오류:이 컴퓨터의 규칙이 일치 하지 않습니다.

이 알려진 문제의 업데이트 된 상태를 확인 하려면 [이 컴퓨터의 규칙이 Microsoft Exchange의 규칙과 일치 하지 않음](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) 을 참조 하십시오.

Outlook 팀은 12928.10000 빌드에 수정 사항을 구현 했습니다. 수정 프로그램은 이미 초기 참가자에 게 빠르게 전달 되며 6 월 2020 일 후반에 월별 채널로 이동 합니다. 빌드를 고정 한 후에는 마지막으로 어떤 규칙을 유지할지 확인 하 라는 메시지가 표시 될 수 있습니다. 메시지가 표시 되 면 서버를 선택한 다음 Outlook에서 다시 이동 하 여 사용 하지 않도록 설정 된 규칙을 다시 사용 하도록 설정 합니다.

수정 프로그램을 사용할 수 있을 때까지 다음 해결 방법을 사용 하십시오.

**해결 방법**: 최근 보고서에서는 Outlook 데스크톱에서 생성 된 클라이언트 규칙만 있는 문제에 대해 문제가 발생 했습니다. 계속 해 서 문제가 발생 하면 규칙을 삭제 한 다음이 문제가 해결 될 때까지 OWA (Outlook Web App)에서 규칙을 만들고 편집 하는 것이 좋습니다.

규칙을 수동으로 삭제할 수 없으면 Outlook을 시작할 때 Outlook.exe/cleanrules를 실행 하 여 Outlook 명령을 실행할 수 있습니다. 이렇게 하면 클라이언트 및 서버 규칙이 모두 삭제 됩니다. Outlook 프로필의 모든 계정에 대 한 모든 규칙이 삭제 됩니다. 이 명령은 명령줄 스위치 문서에 자세히 설명 되어 있습니다.

