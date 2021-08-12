---
title: 응용 프로그램 로그인 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: e1fd31366f24331e74b7e35887c3275549a7a394b128da560ba7a76437979553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925675"
---
# <a name="issues-signing-in-to-applications"></a>응용 프로그램 로그인 문제

원인을 감지하거나 사용자 로그인 관련 문제를 진단하려면 다음 단계를 수행합니다.

1. [로그인 진단](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)을 실행합니다.
2. 사용자, 응용 프로그램, 로그인 시간, 요청 ID 또는 상관 관계 ID에 대한 세부 정보를 입력하여 분석할 이벤트를 찾습니다.
3. 필요한 경우 변경하기 위해 수행할 수 있는 작업과 작업에 대한 세부 정보를 보여주는 진단 결과를 검토합니다.

다음은 응용 프로그램에 로그인할 때 발생할 수 있는 몇 가지 일반적인 문제입니다.

1. 사용자 또는 다른 사용자가 **Azure AD 로그인을 완료했지만 예기치 않은 메시지가 나타나는 경우** [응용 프로그램에 로그인할 때 예기치 않은 동의 프롬프트](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) 및 [응용 프로그램에 대한 동의를 수행할 때 예기치 않은 오류](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error) 문서를 참조하세요.
2. 사용자 또는 다른 사용자가 **응용 프로그램에 직접 로그인했지만 사용자 포털 또는 액세스 패널의 딥 링크에서 응용 프로그램에 로그인할 수 없는 경우** [Azure AD 내 앱에서 응용 프로그램에 로그인하는 문제 해결](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)을 참조하세요.
3. 귀하 또는 사용자가 **Azure AD 로그인을 완료했지만 애플리케이션에 오류 메시지가 표시되고 사용자가 로그인 흐름을 완료할 수 없음**: 문제는 앱이 승인하지 않았다는 것입니다. Azure AD가 발행한 응답입니다. 문제를 해결하려면 [이 단계](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error)를 따르세요.
4. 사용자 또는 다른 사용자가 **암호 Single Sign-On에 대해 구성된 비암호 응용 프로그램에 로그인할 수 없는 경우** 문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)의 지침을 따르세요.
5. 사용자 또는 다른 사용자가 **암호 Single Sign-On에 대해 구성된 Azure AD 암호 응용 프로그램에 로그인할 수 없는 경우** 문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)의 지침을 따르세요.
6. 사용자나 다른 사용자가 **Microsoft 응용 프로그램에 로그인할 수 없는 경우** 문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)를 따르세요.
7. 사용자 또는 다른 사용자가 **암호 Single Sign-On에 대해 구성된 비암호 응용 프로그램에 로그인할 수 없는 경우** 문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery)의 지침을 따르세요.
8. 사용자 또는 다른 사용자가 **암호 Single Sign-On에 대해 구성된 Azure AD 암호 응용 프로그램에 로그인할 수 없는 경우** 문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)의 지침을 따르세요.
9. 사용자나 다른 사용자가 **사용자가 개발한 응용 프로그램에 로그인할 수 없는 경우** 문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)를 따르세요.
10. 사용자 또는 다른 사용자가 **Azure AD 응용 프로그램 프록시를 사용하여 온-프레미스 응용 프로그램에 로그인할 수 없는 경우** 문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy)를 따르세요.

