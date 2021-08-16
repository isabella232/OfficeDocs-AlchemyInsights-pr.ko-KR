---
title: 알림 AAD 커넥트
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
- "9003245"
- "9326"
ms.openlocfilehash: b8713700ee4fc8863a269c99b92954e1df45e1e647c491fb9b439ab83c49f2ff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097312"
---
# <a name="notification-aad-connect"></a>알림 AAD 커넥트

- 작업을 수행할 수 있는 권한이 부여된지 확인 전역 관리자는 기본적으로 액세스할 수 있습니다. 또한 역할 기반 액세스 [제어를](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) 사용하여 참가자에게 등록 권한을 위임할 수 있습니다.
- 필요한 끝점이 사용하도록 설정되어 있으며 방화벽으로 인해 차단되지 않는지 확인합니다. 자세한 내용은 요구 사항을 [참조하세요.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- 네트워크 계층에 의해 SSL 검사가 진행되는 아웃바운드 통신으로 인해 등록이 실패할 수 있습니다.
- Azure AD 2013의 알림 설정을 확인한 커넥트 설정을 검토합니다. Azure AD 및 상태 알림에 대한 알림 설정을 커넥트 방법을 이해하려면 이 가이드를 [참조하세요.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)
- AAD 커넥트 상태 동기화 보고서 및 다운로드 방법에 대한 자세한 내용은 개체 수준 동기화 보고서 [를 참조합니다.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

AAD 커넥트 상태 경고 문제를 해결하기 위해 [AAD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) 커넥트 상태 데이터 상태 알림 문제 해결 가이드를 따르고 일반적으로 묻는 질문은 [Common AAD 커넥트 Health installation questions을](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)참조하십시오.
