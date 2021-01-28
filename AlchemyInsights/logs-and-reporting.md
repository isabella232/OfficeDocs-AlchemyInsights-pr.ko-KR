---
title: 로그 및 보고
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50031501"
---
# <a name="logs-and-reporting"></a>로그 및 보고

[Azure Active Directory 보고 FAQ는](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) Azure AD(Azure Active Directory) 보고에 대한 질문과 대답입니다. 자세한 내용은 [Azure Active Directory 보고를 참조하세요.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)

**감사 문제 해결**

1. 일부 감사 활동이 표시하는 데 문제가 있으며 누락된 활동이 이 목록에 있는 경우 [지원](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)티켓을 제출하세요.
2. 테넌트에 감사 로그가 표시하는 데 문제가 있는 경우 지원 티켓을 제출하세요.
3. Azure Portal에 감사 활동이 즉시 표시되지 않는 [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) 경우 지연이 문서화된 대기 시간을 초과하는 경우 대기 시간 정보를 확인하고 지원 티켓을 제출하세요.
4. [Azure AD 활동 로그 보존](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. 선택한 날짜 범위에 대한 모든 감사가 표시되지 않는 경우 Azure Portal에서 최대 250K 행(가장 최근의 순서로 정렬)의 로그인을 다운로드할 수 있습니다. 자세한 내용은 감사 활동 [다운로드를 참조하세요.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)

**로그인 문제 해결**

1. 테넌트에 대한 Azure AD Premium(P1 또는 P2) 라이선스가 있는 경우 지난 30일간의 데이터만 볼 수 있습니다.
2. 로그인은 Azure AD Premium 테넌트에만 사용할 수 있습니다. 무료 또는 기본 라이선스 테넌트에는 사용할 수 없습니다.
3. 테넌트에 Premium P1 라이선스가 있는 경우 로그인을 볼 수 없는 [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) 경우 지연 시간이 문서화된 대기 시간을 초과하는 경우 대기 시간 정보를 확인하고 지원 티켓을 제출하세요.
4. 선택한 날짜 범위에 대한 모든 로그인이 표시되지 않는 경우 Azure Portal에서 최대 250K 행(가장 최근으로 정렬)의 로그인을 다운로드할 수 있습니다. 자세한 내용은 로그인 활동 [다운로드를 참조하세요.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)

**보안 보고서 문제 해결(위험에 플래그가 지정되어 있는 사용자, 위험한 로그인)**

1. [위험 보안 보고서에 플래그가 지정된 사용자](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [Azure Active Directory 포털의 위험한 로그인 보고서](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [Azure Active Directory 위험 이벤트](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
