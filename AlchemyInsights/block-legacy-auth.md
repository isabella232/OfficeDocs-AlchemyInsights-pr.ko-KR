---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820184"
---
# <a name="blocking-legacy-authentication"></a>레거시 인증 차단

레거시 인증은 다음에서 수행한 인증 요청을 참조하는 용어입니다.

- 최신 인증을 사용하지 않는 이전 Office 클라이언트(예: Office 2010 클라이언트)

- IMAP/SMTP/POP3와 같은 레거시 메일 프로토콜을 사용하는 모든 클라이언트.

레거시 인증 차단 및 최신 인증 사용에 대한 자세한 내용은 레거시 인증 [차단을 참조하세요.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)

Azure AD(Azure Active Directory)의 보안 기본값을 사용하면 보안이 강화되어 조직을 보호할 수 있습니다. 보안 기본값에는 일반적인 공격에 대해 미리 구성한 보안 설정이 포함되어 있습니다.
보안 기본값에 대한 자세한 내용은 [보안 기본값이란?을 참조하세요.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) 

**참고:** 테넌트가 2019년 10월 22일 또는 그 이후에 만들어진 경우 새로운 보안 기본 동작이 발생하고 테넌트에서 보안 기본값이 이미 활성화되어 있는 것일 수 있습니다.  모든 사용자를 보호하기 위해 만들어진 모든 새 테넌트에 보안 기본값이 롤아웃됩니다.
