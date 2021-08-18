---
title: Edge 브라우저를 사용하여 표시기가 작동하지 않음
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: 2a48a49ec52a585e450edf448bc9203cd9c3f935
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326267"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Edge 브라우저를 사용하여 표시기가 작동하지 않음

표시기를 만든 후에는 Edge(Smartscreen)가 표시기를 사용할 수 없습니다. 자세한 내용은 [IP 및 URL/도메인 표시기 생성](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)을 참조하세요.

## <a name="step-1-ensure-the-following"></a>1단계: 다음을 확인하세요.

- 표시기가 올바른지 확인합니다(IP/URL에 오타가 없는지, 올바른 동작, 올바른 RBAC 그룹).
- 표시기를 만든 후 가능한 대기 시간을 고려하여 최소 2시간 동안 기다립니다.
- 시스템이 엔드포인트용 Microsoft Defender에 온보드되어 있는지 확인합니다.
- 시스템이 클라우드와 통신할 수 있는지 확인합니다.
- [테스트 사이트](https://demo.smartscreen.msft.net)로 이동하여 Smartscreen이 활성화되어 있고 연결할 수 있는지 확인합니다.

## <a name="step-2-troubleshoot-the-potential-issue"></a>2단계: 잠재적인 문제를 해결합니다.

- 클라이언트가 요구 사항을 충족하는지 확인합니다. 자세한 내용은 [IP 및 URL/도메인에 대한 지표 만들기](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)를 참조하세요.
- Edge 브라우저의 최신 버전을 실행 중인지 확인합니다. 최신 버전을 찾으려면 [내 Microsoft Edge 버전 확인](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)을 참조하세요.
- Edge 브라우저를 다시 시작합니다.
- 표시기를 설정한 사이트로 이동합니다. 사이트가 예상대로 표시되지 않으면 3단계로 계속 진행합니다. 

## <a name="step-3-collect-data"></a>3단계: 데이터를 수집합니다.

- **MDEClientAnalyzer** 진단 데이터를 수집합니다. 자세한 내용은 [엔드포인트용 Microsoft Defender로 시스템 온보드 문제 해결](issues-with-onboarding-machines.md)을 참조하세요.
- Fiddler 트레이스를 설치하고 수집하는 데 불편함이 없는 경우 [Telerik Fiddler](http://www.telerik.com/fiddler)를 참조하세요.
- Microsoft 지원의 지침을 원하는 경우 아래 지원 아이콘을 선택하여 지원 사례를 여세요.
