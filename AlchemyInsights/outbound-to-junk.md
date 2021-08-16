---
title: 정크 메일 폴더로의 아웃바운드 전자 메일
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 52aa5aa86848fa92ac082e8f672f9f501cd97cf2f3db9c40fa745aa8ebccfbb1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54096664"
---
# <a name="outbound-email-to-junk-email-folder"></a>정크 메일 폴더로의 아웃바운드 전자 메일

아웃바운드 메시지가 정크로 표시된 경우 다음 단계를 수행합니다.

- 아직 없는 경우 아웃바운드 스팸 정책 알림 을 [구성하는 방안을 고려합니다.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)

- 메시지 [추적을](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) 사용하여 아웃바운드 메시지에 추가 세부 정보가 있는 스팸 이벤트 값이 **스팸인지** 확인: 높은 위험 배달 풀 **사용.**

  이러한 메시지의 경우 메시지 콘텐츠를 확인하여 스팸으로 간주될 수 있는 내용을 확인할 수 있습니다. 예를 들어 서명으로 인해 많은 사용자에게 문제가 발생할 수 있습니다.

  정크 메일로 표시된 합법적인 아웃바운드 메시지의 여러 예가 있는 경우 지원 티켓을 열고 지원 에이전트에게 스팸 분석가에게 메시지를 가짓 긍정으로 제출해 줄 것을 요청합니다. 모든 메시지 헤더가 포함된 샘플 메시지를 제공할 준비를 합니다.
