---
title: 도메인 서비스에 대한 암호 해시 동기화
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 3c00105a67f70ae9ce11cd8bb922c4d84a320010d021414b9159948f7dc87dbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040872"
---
# <a name="password-hash-synchronization-for-domain-service"></a>도메인 서비스에 대한 암호 해시 동기화

**Azure AD DS 인스턴스에 암호 해시 동기화를 사용하도록 설정하라는 메시지가 표시될 경우**

사용자가 온-프레미스 Azure AD DS(도메인 서비스) 환경에서 동기화하는 하이브리드 환경을 실행하는 시나리오가 발생할 수 있습니다. 이 시나리오는 온-프레미스 AD DS에서 Azure AD 테넌트로 암호 해시 동기화가 있는 경우 발생됩니다.

**원인**

Azure AD Connect는 기본적으로 Azure AD DS에 필요한 레거시 새 기술 LAN 관리자(NTLM) 및 Kerberos 암호 해시를 동기화하지 않습니다.

**해결 방법** 

NTLM 및 Kerberos 인증에 필요한 암호 해시를 동기화하려면 Azure AD Connect를 구성해야 합니다.

Azure AD Connect가 구성된 후에는 온-프레미스 계정 만들기 또는 암호 변경 이벤트도 Azure AD에 레거시 암호 해시를 동기화합니다. Azure AD DS 하이브리드 환경에서 암호 동기화를 설정하는 방법에 대한 지침은 [여기](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync)를 참조하세요.