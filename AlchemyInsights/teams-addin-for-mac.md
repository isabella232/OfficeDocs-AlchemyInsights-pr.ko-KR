---
title: Mac용 Teams 추가 기능
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2020
ms.locfileid: "46617104"
---
# <a name="teams-add-in-for-mac"></a>Mac용 Teams 추가 기능

누락된 Mac 운영 체제 사용자의 Teams 추가 기능 문제를 해결하려면 다음 단계를 수행합니다.

**1단계:** 하이브리드 Exchange On-Premises(2016 CU3  이상 필요)가 있는 경우 Test-HMA.ps1 도구를 사용하여 Hybrid Modern Authentication이 올바르게 구성되었는지 확인합니다. 자세한 내용은 [iOS 및 Android용 하이브리드 현대 인증 설정](https://aka.ms/AA980zq)을(를) 참조하시기 바랍니다.  

**참고** domain\username이 아닌 UPN 주소 형식(예: [username@contoso.com](mailto:username@contoso.com))을 사용합니다. Exchange Online 사서함을 사용하는 사용자에게도 이 작업을 수행합니다.

**2 단계:** 사용자가 Mac용 Outlook에서 **도구** > **계정**으로 이동하고 계정을 찾아서 선택하도록 합니다. 나열된 사용자 이름이 UPN 형식인지 확인합니다(예: [username@contoso.com](mailto:username@contoso.com)).

**3단계:** 사용자가 라이센스가 부여된 Microsoft Teams 사용자인지 확인합니다. 사용자는 Mac용 Office 365 제품 버전 16.24 이상을 사용해야 합니다.