---
title: 동기화된 사용자 관리
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
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823973"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>기본 전자 메일 주소를 설정하거나, 사용자 특성을 변경하거나, 동기화된 사용자를 제거/삭제할 수 없습니다.

사용자 환경에 대해 디렉터리 동기화를 사용하도록 설정한 경우 Microsoft 365 관리 센터를 사용하여 일부 사용자 또는 개체 특성을 변경할 수 없습니다.

동기화된 사용자와 모든 특성을 완전히 관리하기 위해 로컬 Active Directory 사용자 및 그룹 관리 콘솔(adsiedit.msc)을 사용하세요.  

또는 다음과 같은 일반적인 예와 같이 powershell을 사용하여 동기화된 사용자의 개별 사용자 또는 특성을 변경할 수 있습니다.

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
