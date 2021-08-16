---
title: AllowSelfServicePurchase 정책을 설정하거나 볼 수 없습니다.
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
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020198"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>AllowSelfServicePurchase 정책을 설정하거나 볼 수 없습니다.

AllowSelfServicePurchase 정책을 설정하거나 확인하려고 하면 다음 오류 메시지가 표시됩니다.

*HandleError : PolicyId 'AllowSelfServicePurchase', ErrorMessage를 사용하여 제품 정책을 검색하지 못했습니다. - 연결이 닫혔습니다. 보내기 시 예기치 않은 오류가 발생했습니다.*

이전 버전의 TLS(전송 계층 보안) 때문일 수 있습니다. MSCommerce 서비스를 연결하려면 TLS 1.2 이상을 사용해야 합니다.  

다음 단계를 수행하여 TLS 프로토콜을 1.2로 설정하고 확인한 후 다시 시도합니다.
 1. PowerShell 명령 프롬프트(PS C: 다음 명령을 입력하여 TLS 프로토콜을 버전 \) 1.2로 설정)

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. 다음 명령을 사용하여 사용 중인 TLS 프로토콜을 검증합니다.

    `[Net.ServicePointManager]::SecurityProtocol` 

3. 필요한 경우 Get 또는 Update 명령을 다시 시도합니다.

