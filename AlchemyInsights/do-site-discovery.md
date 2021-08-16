---
title: 사이트 검색 시작
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
- "9143"
- "9005291"
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030764"
---
# <a name="do-site-discovery"></a>사이트 검색 시작

조직에서 여전히 기존 웹 응용 프로그램을 사용하고 있고 Internet Explorer 모드(대부분의 고객이 사용하는)를 사용할 계획이면 몇 가지 추가 사이트 검색을 수행해야 합니다.

**이전 버전의 Microsoft Edge를 배포한 경우**

이전 버전의 Microsoft Edge에서 작동하도록 엔터프라이즈 사이트 목록을 이미 구성한 경우 사이트 검색이 거의 완료된 것입니다. 중립 사이트를 추가해야 할 수도 있습니다.

중립 사이트는 일반적으로 SSO(Single Sign-On)를 제공하는 사이트입니다. Microsoft Edge에서 중립 사이트로 이동하는 경우 Microsoft Edge에 남아 인증하려고 합니다. Internet Explorer 모드에서 중립 사이트로 이동하는 경우 Internet Explorer 모드로 유지하여 인증하려고 합니다.

사용하는 SSO 또는 기타 중립 사이트를 식별하여 기업 사이트 목록에 추가합니다.

**Internet Explorer가 기본 브라우저로 지정된 경우**

Internet Explorer를 사용하고 있는 경우 최신 웹 표준으로 업그레이드한 사이트와 Internet Explorer가 여전히 필요한 사이트를 모를 수 있습니다. 이러한 사이트에서만 Internet Explorer 모드를 사용할 수 있도록 이러한 사이트를 찾아서 기업 사이트 목록에 추가할 수 있습니다.

> [!NOTE]
> [엔터프라이즈 사이트 검색](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery)은 Internet Explorer 모드가 필요할 수 있는 사이트를 검색합니다. Windows 10, Windows 8.1 또는 Windows 7의 Internet Explorer 11을 통해 Windows Internet Explorer 8을 실행하는 시스템에 대한 데이터를 수집할 수 있습니다.

**데이터 분석**

사이트 데이터를 수집한 후에는 다음 4단계 프로세스를 통해 데이터를 분석하는 것이 좋습니다.
1. 도메인별로 데이터를 정렬한 다음 URL별로 정렬합니다.
2. Internet Explorer 모드에 대해 구성할 앱의 경계를 정의합니다. 앱을 정의하는 모든 사이트 및 웹 컨트롤을 포함하려고 하지만 추가 사이트 및 컨트롤은 포함하지 않습니다. 일부 사이트는 *https://contoso.com/app1* 처럼 단순할 수 있지만 다른 사이트는 여러 사이트와 페이지를 정의해야 할 수도 있습니다.
3. 앱을 테스트하여 기본적으로 작동하지 않는지 확인합니다. 많은 사이트에서 최신 브라우저를 검색할 때 최신 콘텐츠를 제공하고 Internet Explorer를 검색할 때만 기존 콘텐츠를 제공합니다.
4. 테스트에 실패한 경우 엔터프라이즈 사이트 목록에 앱을 추가합니다.

> [!NOTE]
> 앱을 구성하는 모든 사이트를 그룹화하는 것이 좋습니다. 이렇게 하면 앱을 업그레이드할 때 Internet Explorer 모드에서 전체 사이트를 제거하고 해당 앱에 대한 최신 브라우저를 사용하는 것이 더 쉽습니다.

사이트 검색을 완료하고 데이터를 분석했으면 채널 전략을 살펴볼 준비가 되었습니다.

