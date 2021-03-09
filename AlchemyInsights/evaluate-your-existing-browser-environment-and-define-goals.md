---
title: 기존 브라우저 환경을 평가하고 목표 정의
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530129"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a>기존 브라우저 환경을 평가하고 목표 정의

시간을 내어 현재 브라우저 상태와 프로젝트 비전을 파악하면 모든 프로젝트 이해관계자가 조정되고 동일한 목표를 추구할 수 있습니다. 다음 단계를 따르세요.

1. 현재 상태를 정의합니다. 다음과 같은 사항을 고려해야 합니다.
- 현재 환경에 배포된 브라우저는 무엇인가요?
- 어떤 브라우저가 기본 브라우저로 설정되어 있나요?
- 일부 앱에서 Internet Explorer를 사용해야 하나요?
- 현재 엔터프라이즈 모드 사이트 목록을 사용하여 Internet Explorer를 구성하나요?
- 환경이 Windows 10 및 macOS 등 어떤 OS 플랫폼을 지원하나요?
- 브라우저 관리에 어떤 관리 도구를 사용하나요?
- 브라우저 구성 및 관리를 담당하는 사람은 누구인가요?
- 브라우저 호환성을 검증하기 위한 프로세스는 무엇인가요?
2. 배포의 목표를 정의합니다. 다음 사항도 유의해야 합니다.
- [Microsoft Edge를 기본 브라우저로 설정](https://docs.microsoft.com/DeployEdge/edge-default-browser)하고 싶나요?
- Microsoft Edge의 레거시 버전을 숨기고 싶나요? 아니면 [다른 사용자가 사용할 수 있도록 그대로](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge) 두시겠어요?
- [Microsoft Edge를 어떻게 구성](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)할 예정인가요?
- 초기 배포의 일부로 구성하는 데 중요한 기능은 무엇인가요?
- 식별된 호환성 또는 구성 문제를 해결하기 위한 프로세스는 무엇인가요?
3. 다음과 같이 사용하려는 기능에 대한 필수 구성 요소를 이해하세요.
- [Windows Defender Application Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [Internet Explorer 모드](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [인증 및 동기화](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

이러한 단계를 완료하고 나면 배포 전략을 계획할 준비가 된 것입니다.
