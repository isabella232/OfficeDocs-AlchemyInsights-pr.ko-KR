---
title: Microsoft Defender for Endpoint에 컴퓨터 온보딩 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 5f2ed08e32694a6d7293abbabb1eddd3d251ceddbd9debf6ec3143bb4fed86db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054696"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a>Microsoft Defender for Endpoint에 컴퓨터 온보딩 문제

MDE 서비스에 컴퓨터를 온보딩하는 데 문제가 있을 수 있습니다. 최종 사용자 컴퓨터에 액세스할 수 있는 경우 다음 단계를 수행합니다.

1. 최신 미리 보기 버전의 [MDE 클라이언트 분석기](https://aka.ms/betamdeanalyzer) 진단 도구를 다운로드합니다.
2. **MDEClientAnalyzer.cmd** 를 마우스 오른쪽 단추로 클릭하고 ‘관리자 권한으로 실행’을 선택합니다.
3. **MDEClientAnalyzer.htm** 의 제안된 지침을 따릅니다.
4. 자세한 로그는 **MDEClientAnalyzerResult** 라는 하위 폴더를 검토하세요.
5. 추가 지침이 필요한 경우, [엔드포인트용 Microsoft Defender 지원](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support)에 문의하고 분석을 위해 결과 MDEClientAnalyzerResult.zip 파일을 제공합니다.
