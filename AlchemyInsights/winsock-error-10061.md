---
title: 1554 Winsock 오류 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083236"
---
# <a name="winsock-error-10061"></a>Winsock 오류 10061

이 오류 코드는 Microsoft가 대상 호스트와 TCP 소켓(연결)을 설정할 수 없습니다. 이 오류의 가장 일반적인 원인은 방화벽 구성 문제입니다. 문제를 해결하려면 다음 설정을 확인합니다.

- URL 및 IP 주소 범위에 Microsoft 365 방화벽 구성 [확인](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- 오류가 EOP(Exchange Online Protection)와 관련이 있는 경우 이전에 해당 IP 주소의 변경 [Exchange Online Protection 합니다.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- ISP(인터넷 서비스 공급자)가 포트를 차단하지 않는지 확인합니다.

- 커넥터에서 스마트 호스트 및 대상 서버 설정을 확인합니다.

이 Microsoft 365 들어오는 연결을 차단하지  않습니다.
