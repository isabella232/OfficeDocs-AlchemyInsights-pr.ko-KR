---
title: MFA 관련 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810490"
---
# <a name="issues-with-azure-mfa"></a>Azure MFA 관련 문제
사용자가 MFA(다단계 인증)를 사용하여 로그인할 수 없는지 확인할 수 있는 몇 가지가 있습니다.

1. 영향을 받는 사용자는 Azure Active Directory 포털에서 차단될 수 있습니다. 이 경우 해당 특정 사용자에 대한 인증 시도가 자동으로 거부됩니다. [이 문서의 단계에 따라 차단을 해제하세요.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. 사용자의 차단 해제가 도움이 되지 않았거나 사용자가 차단되지 않은 경우 사용자의 MFA를 다시 설정하려고 시도할 수 있으며 등록 프로세스를 다시 거치게 됩니다. [이 문서의 단계를 따르세요.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

MFA를 처음 사용하도록 설정한 경우 사용자가 Outlook, Skype 등의 비 브라우저 클라이언트에 로그인할 수 없는 경우 O365 구독에서 ADAL(Active Directory 인증 라이브러리)을 사용할 수 없습니다. 이 경우 Exchange Online Powershell에 연결하고  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*