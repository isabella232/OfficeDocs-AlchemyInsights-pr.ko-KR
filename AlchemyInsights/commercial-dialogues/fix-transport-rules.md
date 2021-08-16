---
title: 전송 규칙 수정
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034760"
---
# <a name="fix-transport-rules"></a>전송 규칙 수정

사용자 지정 메일 흐름 규칙이 이 메시지에 영향을 주었다. 정확한 규칙을 검토하기 위해 다음을 합니다.

1. 제출 결과의 **추가 정보 아래에서** **GUID** 또는 정책 이름을 **메모합니다.**
2. 관리 Exchange 실행합니다. 자세한 내용은 [Open the Exchange Management Shell 을 참조하십시오.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. 다음 명령을 실행합니다(제출의 GUID 사용): **Get-TransportRule -identity "GUID"** | fl * Description*
4. 설명을 검토하여 메시지에 영향을 주는 구성된 조건을 검토합니다.

자세한 내용은 [Get-TransportRule 을 참조합니다.](https://go.microsoft.com/fwlink/?linkid=2101523)
