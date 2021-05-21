---
title: Mac용 Teams 추가 기능
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582076"
---
# <a name="teams-add-in-for-mac"></a>Mac용 Teams 추가 기능

누락된 Mac 운영 체제 사용자의 Teams 추가 기능 문제를 해결하려면 다음 단계를 수행합니다.

**1단계:** 하이브리드 Exchange On-Premises(2016 CU3  이상 필요)가 있는 경우 Test-HMA.ps1 도구를 사용하여 Hybrid Modern Authentication이 올바르게 구성되었는지 확인합니다. 자세한 내용은 [iOS 및 Android용 하이브리드 현대 인증 설정](https://aka.ms/TestHMAEAS)을(를) 참조하시기 바랍니다.  

**참고** domain\username이 아닌 UPN 주소 형식(예: [username@contoso.com](mailto:username@contoso.com))을 사용합니다. Exchange Online 사서함을 사용하는 사용자에게도 이 작업을 수행합니다.

**2 단계:** 사용자가 Mac용 Outlook에서 **도구** > **계정** 으로 이동하고 계정을 찾아서 선택하도록 합니다. 나열된 사용자 이름이 UPN 형식인지 확인합니다(예: [username@contoso.com](mailto:username@contoso.com)).

**3단계:** 사용자가 라이센스가 부여된 Microsoft Teams 사용자인지 확인합니다. 사용자는 Mac용 Office 365 제품 버전 16.24 이상을 사용해야 합니다.