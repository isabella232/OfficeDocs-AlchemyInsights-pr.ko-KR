---
title: Office 365용 Microsoft Defender 안전 첨부 파일 정책 예
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736749"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Office 365용 Microsoft Defender 안전 첨부 파일 정책 예

이러한 설정을 사용하면  메시지를 즉시 배달하는 지연 없음이라는 정책을 사용하도록 설정한 다음 첨부 파일을 검사한 후 다시 연결합니다.

- **이름:** 지연 없음
- **설명:** 메시지를 즉시 배달하고 검사 후 첨부 파일을 다시 연결합니다.
- **응답:** 동적 배달 **옵션을** 선택합니다. 자세한 내용은 안전 첨부 파일 [정책의 동적 배달을 참조하세요.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **첨부 파일** 리디렉션 섹션: 리디렉션을 사용하도록 설정 옵션을 선택한 다음 악의적인 첨부 파일을 조사할 Microsoft 365 전역 관리자, 보안 관리자 또는 보안 분석가의 전자 메일 주소를 입력합니다.
- **적용 대상** 섹션: 받는 사람 도메인이 입니다.를 **선택한** 다음 도메인을 선택합니다. **추가를** 선택한 다음 확인 을 **선택합니다.** 완료되면 저장을 **선택합니다.**

자세한 내용은 [Microsoft Defender for Office 365의](https://go.microsoft.com/fwlink/?linkid=2092213)안전한 첨부 파일을 참조합니다.
