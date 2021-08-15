---
title: 예기치 않은 다단계 인증
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: d2b97175049bd9732b7444b029f7ea8610c3d5a2c02878ec5f20ded916baadd5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53991145"
---
# <a name="unexpected-multi-factor-authentication"></a>예기치 않은 다단계 인증

2019년 10월 21일 이후에 테넌트를 생성했으며 MFA에 대한 메시지가 예기치 않게 표시될 경우 테넌트에서 [보안 기본값](https://aka.ms/securitydefaults)이 사용하도록 설정되어 있을 수 있습니다. 

보안 기본값을 관리하려면:

1. 전역 관리자 자격 증명을 사용하여 [관리 센터](https://go.microsoft.com/fwlink/p/?linkid=834822)에 로그인합니다.

2. [Azure Active Directory 속성](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)으로 이동합니다.

3. 페이지 맨 아래에서 **보안 기본값 관리** 를 클릭합니다.

4. 보안 기본값을 사용하도록 설정하려면 **예** 를 클릭하고 사용하지 않도록 설정하려면 **아니요** 를 클릭합니다.
