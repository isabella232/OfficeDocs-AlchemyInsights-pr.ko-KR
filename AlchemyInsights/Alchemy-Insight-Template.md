---
title: 파일 이름과 가장 같아야 합니다.
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 7b915ab18d10948b8588dc6e2ef6af9891524861a924e2193dd73c2c77ffe6da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918901"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"필수 연금술 헤더 H1, H2가 작동하지 않습니다."
연산 제작에 대한 모범 사례 및 지침:

1. 폴더에 Insights 연금술을 **중첩하지 않습니다.** 이렇게 하면 URL 구조가 중단됩니다. We're looking into fixing this.
1. **AlchemyInsights** 폴더의 파일에는 공백에 대한 하이픈이 있는 소문자 파일 이름을 지정해야 합니다. **_how-to-enable-litigation-hold_**.
    1. ms.custom 필드에 연금 파트너 [](https://alchemyportal.azurewebsites.net) 포털의 규칙 ID 또는 버킷 ID를 포함합니다. ex. ***ms.custom: 100021***
1. 이 파일의 맨 위에 있는 나머지 메타데이터를 템플릿으로 사용 합니다.
1. 연산 파트너 [포털에서](https://alchemyportal.azurewebsites.net)고객 인사이트 **제목:** 섹션으로 이동하여 인사이트를 위한 H1 타이틀의 시작점으로 활용합니다. 
    > [!NOTE]
    > 연금 Insights 맨 위에는 H1이 하나만 있어야 합니다. 아니면 프로덕션에서 중단됩니다. H2는 렌더링되지 않습니다. 따라서  굵게 또는 다른 규칙을 사용하여 개별 섹션을 의미합니다.
1. 다음으로, 연산 규칙 페이지의 Customer Insights 초안 자료를 사용하여 본문을 채우기
    1. 글머리 기호 목록이 괜찮습니다.
    1. 번호 매기기 목록도
    1. **굵게** *및 Italic은* 확인입니다.
    1. 링크는 항상 내부 링크가 아닌 **"웹에 대한 링크"/외부** **또는 UI** 요소에 대한 딥 링크입니다.
    1. 현재 그림은 공식적으로 지원되지 않지만 로드맵에 있습니다.

이 시간이 너무 늦습니다. 모범 사례는 약 400자 ---------------------------------

콘텐츠가 준비되면 라이브 분기로 끌어오기. 그런 다음 연산 파트너 포털로 [이동하여](https://alchemyportal.azurewebsites.net) url 필드에 파일 이름을 입력합니다. 