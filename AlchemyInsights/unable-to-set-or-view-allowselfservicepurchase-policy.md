---
title: AllowSelfServicePurchase 정책을 설정 하거나 볼 수 없습니다.
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735205"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>AllowSelfServicePurchase 정책을 설정 하거나 볼 수 없습니다.

AllowSelfServicePurchase 정책을 설정 하거나 확인 하려고 하면 다음과 같은 오류 메시지가 나타납니다.

*HandleError: PolicyId가 ' AllowSelfServicePurchase ' 인 제품 정책을 검색 하지 못했습니다. ErrorMessage-기본 연결이 닫혔습니다. 보내기에서 예기치 않은 오류가 발생 했습니다.*

이전 버전의 TLS (전송 계층 보안)로 인 한 것일 수 있습니다. MSCommerce 서비스에 연결 하려면 TLS 1.2 이상을 사용 해야 합니다.  

다음 단계를 수행 하 여 TLS 프로토콜을 1.2으로 설정 하 고 확인 하 고 다시 시도 합니다.
 1. PowerShell 명령 프롬프트 (PS C: \) 다음 명령을 입력 하 여 TLS 프로토콜을 버전 1.2으로 설정 합니다.

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. 다음 명령을 사용 하 여 사용 중인 TLS 프로토콜을 확인 합니다.

    `[Net.ServicePointManager]::SecurityProtocol` 

3. 필요에 따라 가져오기 또는 업데이트 명령을 다시 시도 합니다.

