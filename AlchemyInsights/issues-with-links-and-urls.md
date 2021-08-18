---
title: 링크 및 URL 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: d85069970fe6bc6cc7a8488c49c0e6236426d45b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321913"
---
# <a name="issues-with-links-and-urls"></a>링크 및 URL 문제

리디렉션 URI/회신 URL(두 표현은 모두 교환 가능)은 Microsoft ID 플랫폼에서 앱 요청 토큰을 반환하는 데 사용되는 URL입니다. 이러한 URL에 대한 자세한 내용은 다음 문서를 참조하세요.

- [인증 흐름 및 응용 프로그램 시나리오](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - 각 시나리오에 대한 **앱 등록** 페이지의 리디렉션 URI에 대한 정보입니다.
- [리디렉션 URI/회신 URL 제한사항 및 한계](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**앱에 대한 올바른 리디렉션 URI/회신 URL을 등록하는 방법을 모르는 경우**

개발 중인 응용 프로그램으로 로그인할 때 로그인 대화 상자에 **AADS50011이 표시되는 경우: 요청에 지정된 응답 URL이 응용 프로그램 <your app ID>** 에 대해 구성된 응답 URL과 일치하지 않습니다. 응용 프로그램 등록에 코드를 사용하여 Microsoft ID 플랫폼에 요청한 리디렉션 URI를 추가해야 합니다.

회신 URL을 추가하기 위해 Azure Portal의 **응용 프로그램 등록** 페이지에서 **인증** 탭으로 이동한 다음 **리디렉션 URI** 섹션에 항목을 추가합니다. 입력해야 하는 값은 아래 설명된 바와 같이 구축하는 응용 프로그램의 유형에 따라 다릅니다.

- 단일 페이지 응용 프로그램 및 웹앱의 경우 회신 URL은 응용 프로그램의 URL입니다. [단일 페이지 응용 프로그램 등록](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) 또는 [Azure Portal을 사용하여 웹 응용 프로그램 등록](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)을 참조하십시오.
- 데스크톱 앱의 경우 선택해야 하는 값은 다음에 따라 선택해야 합니다.
    - 플랫폼(MacOS는 Windows 또는 버전과 다를 수 있습니다.)
    - 통합 Windows 인증 [IWA] 또는 사용자 이름/암호를 사용하여 장치 코드 흐름을 통해 대화형 토큰을 획득하는 방식입니다.
    자세한 내용은 [데스크톱 앱 - 앱 등록 - 리디렉션 URi를 참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- 모바일 응용 프로그램의 경우 리디렉션 URI는 다음에 따라 다를 수 있습니다.
    - 플랫폼(iOS/Android/UWP)
    - iOS의 번들 ID와 같은 앱을 빌드하는 데 사용되는 정보와 Android Azure Portal 앱 등록의 패키지 이름 및 서명 해시가 도움이 됩니다. 자세한 내용은 [플랫폼 구성 및 리디렉션 URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)를 참조하세요.

**참고**: 웹 API 및 IWA(사용자 이름/암호)를 자동으로 사용하는 일부 방법은 리디렉션 URI가 필요하지 않습니다.

**웹 응용 프로그램을 배포했습니다. 배포된 앱을 테스트할 때 회신 URL 불일치 메시지가 나타나는 경우**

웹 응용 프로그램을 배포하는 모든 위치에 대한 리디렉션 URI를 추가합니다. 자세한 내용은 [Azure Portal을 사용하여 웹앱 앱 등록](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)을 참조하세요.

**참고**: 해당 위치에 응용 프로그램을 배포한 직후 위치에 대한 리디렉션 URI를 추가합니다.

**충분한 회신 URL을 등록할 수 없는 경우**

ISV인 경우 모든 고객에 대해 하나 또는 여러 개의 리디렉션 URI가 있습니다. ADAL/Azure AD v1.0에서 MSAL/Microsoft ID 플랫폼으로 마이그레이션하려는 경우 [리디렉션 URI의 최대 개수](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris)에 도달합니다. 이 문제를 해결하기 위해 [해당하는 서비스에 리디렉션 URI를 추가](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals)합니다.
