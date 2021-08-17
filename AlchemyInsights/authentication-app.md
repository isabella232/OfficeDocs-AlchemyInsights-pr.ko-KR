---
title: 인증 앱
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082948"
---
# <a name="authentication-app"></a>인증 앱

전역 관리자인 경우 로그인 진단 을 사용하여 발생된 문제를 빠르게 찾거나 사용자 로그인과 관련된 문제를 진단할 [수 있습니다.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. "진단 시작" 단추를 클릭하여[진단을](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)시작하세요. 
1. 사용자, 응용 프로그램, 로그인 시간, 요청 ID 또는 상관 관계 ID에 대한 세부 정보를 입력하여 분석할 이벤트를 찾아야 합니다.
1. 필요한 경우 변경하기 위해 수행할 수 있는 작업과 작업에 대한 세부 정보를 보여주는 진단 결과를 검토합니다.

**적용 가능한 시나리오를 검사합니다.**

1. 사용자가 Microsoft Authenticator 앱에서 푸시 알림을 수신하지 않는 경우 사용자 차단 및 차단 해제에 설명된 MFA 차단된 사용자 아래에 해당 사용자가 표시되지 [않는지 확인해야 합니다.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. 사용자가 MFA에 대해 차단되지는 않지만 푸시 알림을 받지 않는 경우 보류 중인 승인 요청을 끌어오는 Microsoft Authenticator 앱을 열 수 있습니다.
1. 다른 로그인 방법으로 로그인을 클릭하고 모바일 앱에서 확인 코드 사용을 선택할 수도 있습니다.
1. Microsoft Authenticator 앱만 사용할 수 있습니다. [보안 기본값에 대해 자세히 알아보고](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) [Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) 자주 묻는 질문과 해결 방법을 확인할 수 있습니다.
 
**권장 비디오**

[새 휴대폰에서 Authenticator 앱을 설정하는 방법(2분)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
