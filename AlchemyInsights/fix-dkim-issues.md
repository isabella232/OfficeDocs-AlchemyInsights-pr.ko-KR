---
title: DKIM 설치 문제 해결
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945937"
---
# <a name="fix-dkim-setup-issues"></a>DKIM 설치 문제 해결

사용자 지정 도메인에 DKIM을 사용하도록 설정하는 데 문제가 있는 경우 다음 단계를 수행합니다.

- 대부분의 DKIM 설치 문제는 잘못된 DNS 레코드와 관련이 있습니다. DKIM CNAME 레코드(TXT 레코드 아님)의 서식이 올바르게 지정되어 있는지 확인합니다. 자세한 내용은 이 항목을 [참조하세요.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- 도메인의 DNS 호스팅 서비스(일반적으로 도메인 등록 기관)에서 DKIM DNS 레코드를 만들거나 업데이트한 후 DNS 레코드가 전파될 때까지 기다렸다가

- 관리 센터에서 DKIM DNS 레코드를 만들 수 없는 경우 사용자 지정 도메인(예: contoso.com)으로 바꾸고 powerShell : 에서 Exchange Online 실행할 수 \<CustomDomain\> [](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` 있습니다.
