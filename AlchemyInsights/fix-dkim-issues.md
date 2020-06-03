---
title: DKIM 설정 문제 해결
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506780"
---
# <a name="fix-dkim-setup-issues"></a>DKIM 설정 문제 해결

사용자 지정 도메인에 대해 DKIM을 사용 하도록 설정 하는 데 문제가 발생 하면 다음 단계를 수행 합니다.

- 대부분의 DKIM 설정 문제는 잘못 된 DNS 레코드와 관련이 있습니다. TXT 레코드가**아닌** DKIM CNAME 레코드의 서식이 올바르게 지정 되었는지 확인 합니다. 자세한 내용은이 [항목](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)을 참조 하십시오.

- 도메인의 DNS 호스팅 서비스 (대개 도메인 등록자)에서 DKIM DNS 레코드를 만들거나 업데이트 한 후에는 DNS 레코드가 전파 될 때까지 기다립니다.

- 관리 센터에서 DKIM DNS 레코드를 만들 수 없는 경우 \<CustomDomain\> 사용자 지정 도메인 (예: contoso.com)으로 대체 하 여 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)에서이 명령을 실행할 수 `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` 있습니다.
