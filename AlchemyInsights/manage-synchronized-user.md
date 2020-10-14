---
title: 동기화 된 사용자 관리
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
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451406"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>기본 전자 메일 주소를 설정 하거나, 사용자 특성을 변경 하거나, 동기화 된 사용자를 제거/삭제할 수 없음

환경에 대해 디렉터리 동기화를 사용 하도록 설정 된 경우에는 Microsoft 365 관리 센터를 사용 하 여 일부 사용자 또는 개체 특성을 변경할 수 없습니다.

동기화 된 사용자 및 모든 해당 특성을 완전히 관리 하려면 로컬 active directory 사용자 및 그룹 관리 콘솔 (adsiedit)을 사용 합니다.  

또는 다음과 같은 일반적인 예와 같이 powershell을 사용 하 여 동기화 된 사용자에 대 한 개별 사용자 또는 특성을 변경할 수 있습니다.

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
