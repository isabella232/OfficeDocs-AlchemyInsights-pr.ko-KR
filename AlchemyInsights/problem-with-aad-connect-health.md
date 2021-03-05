---
title: AAD Connect 상태 문제
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50453295"
---
# <a name="problem-with-aad-connect-health"></a>AAD Connect 상태 문제

- 작업을 수행할 수 있는 권한이 부여된지 확인 전역 관리자는 기본적으로 액세스할 수 있습니다. 또한 역할 기반 액세스 [제어를](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) 사용하여 참가자에게 등록 권한을 위임할 수 있습니다.
- 필요한 끝점이 사용하도록 설정되어 있으며 방화벽으로 인해 차단되지 않는지 확인합니다. 자세한 내용은 요구 사항을 [참조하세요.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- 네트워크 계층에 의해 SSL 검사가 진행되는 아웃바운드 통신으로 인해 등록이 실패할 수 있습니다.
- Azure AD Connect Health에 대한 알림 설정을 확인해야 합니다. 설정을 검토하시기 바랍니다. 이 [가이드는](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) Azure AD Connect 상태 알림에 대한 알림 설정을 구성하는 방법을 이해하는 데 도움이 될 수 있습니다.
- AAD Connect 상태 동기화 보고서 및 다운로드 방법에 대한 자세한 내용은 개체 수준 동기화 [보고서 를 참조합니다.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

AAD Connect 상태 경고 문제를 해결하기 위해 AAD Connect Health [Data Freshness Alerts에](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) 대한 문제 해결 가이드 및 일반적인 질문과 대답을 참조하세요. 일반 AAD Connect Health 설치 질문 을 [참조하세요.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
