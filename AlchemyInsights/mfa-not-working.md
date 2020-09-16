---
title: MFA 문제
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755137"
---
# <a name="issues-with-azure-mfa"></a>Azure MFA 관련 문제
사용자가 MFA (다단계 인증)를 사용 하 여 로그인 할 수 없는지 확인 해야 하는 몇 가지 사항이 있습니다.

1. 영향을 받는 사용자가 Azure Active Directory 포털에서 차단 될 수 있습니다. 이 경우 특정 사용자에 대 한 인증 시도가 자동으로 거부 됩니다. [이 문서에서 설명 하는 단계에 따라 차단을 해제 하세요.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. 사용자가 도움이 되지 않았거나 사용자가 차단 되지 않은 경우 사용자에 대해 MFA를 다시 설정 하 고 등록 프로세스를 다시 진행할 수 있습니다. [이 문서에 나와 있는 단계를 따르세요.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

처음으로 MFA를 사용 하도록 설정 하는 경우 사용자가 Outlook, Skype 등의 비 브라우저 클라이언트에 로그인 할 수 없는 경우에는 O365 구독에서 ADAL (Active Directory 인증 라이브러리)을 사용 하도록 설정 되지 않은 것입니다. 이 경우에는 Exchange Online Powershell에 연결 하 고이 cmdlet을  *set-organizationconfig-OAuth2ClientProfileEnabled: $true* 으로 실행 해야 합니다.