---
title: LDAP 구성
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876571"
---
# <a name="configure-ldap"></a>LDAP 구성

LDAP를 구성하기 위해 다음을 실행합니다.

1. Azure Portal에서 도메인의 [상태 확인](https://aka.ms/aadds-health)
1. 유효한 Azure AD 구독을 사용할 수 있으며 Azure AD 도메인 서비스를 사용하도록 설정되어 있어야 합니다.
1. 보안 LDAP를 사용하도록 설정하는 데 필요한 인증서는 신뢰할 수 있는 공용 인증 기관에서 얻거나 자체 서명된 인증서가 되어야 합니다.
1. 인증서가 필요한 지침을 [따르는지 확인합니다.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**잘못된 인증서**
1. 인증서를 갱신하는 경우 단계에 따라 새 인증서를 만들고 다시 로드합니다. [LDAP 구성.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Azure Active Directory 도메인 서비스에서 보안 LDAP 경고의 알려진 문제를 해결하려면 [LDAP 경고 해결을 참조하세요.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
