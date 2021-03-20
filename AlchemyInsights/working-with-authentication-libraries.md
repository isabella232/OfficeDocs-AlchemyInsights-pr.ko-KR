---
title: 인증 라이브러리 작업
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897899"
---
# <a name="working-with-authentication-libraries"></a>인증 라이브러리 작업

MSAL(Microsoft 인증 라이브러리) 문제를 해결하고 다음 권장 단계를 수행합니다.

1. **MSAL 작업**: [Microsoft ID 플랫폼 인증 라이브러리](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - 이 문서에서는 여러 응용 프로그램 유형에 대한 Microsoft 인증 라이브러리 지원을 보여 줍니다. 여기에는 라이브러리 소스 코드 링크, 앱 프로젝트의 패키지를 가져올 위치, 라이브러리가 사용자 로그인(인증), 보호된 웹 API(인증)에 대한 액세스를 지원하는지 여부 또는 둘 다 포함됩니다.

2. **인증 문제 해결**: MSAL은 여러 응용 프로그램 시나리오에서 사용할 수 있도록 여러 인증 흐름을 지원합니다. 클라이언트 응용 프로그램이 빌드되는 방식에 따라 MSAL은 Microsoft ID 플랫폼에서 지원되는 인증 흐름 중 하나 이상을 사용할 수 있습니다. 이러한 흐름은 여러 유형의 토큰과 인증 코드를 생성할 수 있으며, 이를 작동시키려면 서로 다른 토큰이 필요합니다.

3. **액세스 토큰**: [Microsoft ID 플랫폼 액세스 토큰](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - API에서 액세스 코튼 내부 클레임의 유효성을 검사하고 사용하는 방법을 알아봅니다. 이 게시물의 모든 문서(설명된 경우를 제외)는 등록한 API에 대해 발급된 토큰에만 적용됩니다. Microsoft 소유 API용으로 발급된 토큰에는 적용되지 않으며 사용자가 생성한 API에 대해 Microsoft ID 플랫폼이 토큰을 발행하는 방법을 확인하는 데 이러한 토큰을 사용할 수도 없습니다.

**ADAL(Azure Active Directory 인증 라이브러리)에 대한 지원 종료**

- **2020년 6월 30일부터** ADAL 및 Azure AD Graph에 새로운 기능이 추가되지 않습니다. 기술 지원 및 보안 업데이트를 계속 제공하지만 기능 업데이트는 더 이상 제공하지 않습니다.
- **2022년 6월 30일부터** ADAL 및 Azure AD Graph에 대한 지원을 종료하고 더 이상 기술 지원이나 보안 업데이트를 제공하지 않습니다.
- 기존 OS 버전에서 ADAL을 사용하는 앱은 이 시간 이후에도 계속 작동하지만 *기술 지원이나 보안 업데이트* 를 받지 못합니다.
- 이 시간 이후 Azure AD Graph를 사용하는 앱은 더 이상 Azure AD Graph 끝점에서 응답을 받지 못할 수 있습니다.

**ADAL 마이그레이션**

- 최신 기능 및 보안 업데이트가 있는 MSAL로 업데이트하는 것이 좋습니다.
- Microsoft 앱을 사용하는 경우 Microsoft가 지원 종료시까지 MSAL로 응용 프로그램을 마이그레이션하고 있으며, MSAL의 지속적인 보안 및 기능 개선으로 혜택을 받을 수 있도록 해야 합니다.

1. [ADAL FAQ를 읽어보세요](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [플랫폼별로 앱을 마이그레이션하는 방법을 알아보세요](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. 앱 플랫폼 가이드를 읽은 후 추가 질문이 있는 경우 [azure-addal-declation] 태그가 있는 [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html)에 게시하거나 라이브러리의 GitHub 저장소에서 문제를 열 수 있습니다. 각 라이브러리의 참조 링크는 [MSAL 개요](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) 문서의 **언어 및 프레임워크** 섹션을 참조하세요.
4. **어느 앱에서 ADAL을 사용하는지 이해하는 데 도움이 필요한 경우** 모든 앱의 소스 코드를 검토하는 것이 좋습니다. 해당되는 경우 ISV(독립 소프트웨어 벤더) 또는 앱 공급자에게 문의하세요. 또한 Microsoft 지원을 통해 테넌트에 있는 Microsoft가 아닌 모든 ADAL 앱 목록을 제공할 수 있습니다.







