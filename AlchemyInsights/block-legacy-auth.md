---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685604"
---
# <a name="blocking-legacy-authentication"></a>레거시 인증 차단

레거시 인증은 다음에서 수행한 인증 요청을 참조하는 용어입니다.

- 최신 인증을 사용 하지 않는 이전 Office 클라이언트 (예: Office 2010 클라이언트)

- IMAP/SMTP/POP3와 같은 레거시 메일 프로토콜을 사용하는 모든 클라이언트.

레거시 인증을 차단 하 고 최신 인증을 사용 하는 방법에 대 한 자세한 내용은 [레거시 인증 차단을](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)참조 하십시오.

Azure Active Directory의 보안 기본값 (Azure AD)을 통해 보안을 강화 하 고 조직을 보호 하는 데 도움이 됩니다. 보안 기본값에는 일반적인 공격에 대 한 미리 구성 된 보안 설정이 포함 됩니다.
보안 기본값에 대 한 자세한 내용은 [보안 기본값 이란?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)을 참조 하십시오. 

**참고**: 테 넌 트를 10 월 2 일, 2019 이후에 만든 경우 새 보안 기반 동작이 발생 하 여 이미 테 넌 트에서 보안 기본값을 사용 하도록 설정 했을 수 있습니다.  모든 사용자를 보호 하기 위한 노력의 일환으로, 보안 기본값은 만들어진 모든 새 테 넌 트에 롤아웃 됩니다.
