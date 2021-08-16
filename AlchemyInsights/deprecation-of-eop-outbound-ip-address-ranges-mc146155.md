---
title: 1065 EOP 아웃바운드 IP 주소 범위 사용 안 림C146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031268"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP 아웃바운드 IP 주소 범위 사용 안

조직에서 (2018년 10월 26일까지 수정되지 않은 경우) 메일 흐름이 프레미스 또는 외부 대상에 중단될 수 있는 잠재적인 문제를 감지했습니다. 앞서 설명한 것 처럼 IP 주소 범위 관리를 단순화하기 위해 외부에서 전자 메일을 보내고 받는 데 사용되는 EOP(Exchange Online Protection) IP 주소 범위를 Microsoft 365. 이 분석은 메일 흐름 커넥터에서 구성한 하나 이상의 외부 전자 메일 원본 또는 대상이 여기에 표시된 IP 주소 범위의 연결을 수락하지 않는 것을 [나타냅니다.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

이러한 원본 및 대상이 게시된 모든 EOP IP 주소와의 연결을 수락하도록 10월 26일 [이전의 행동을 합니다.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

이 변경에 대한 자세한 내용은 메시지 센터 게시물 [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)또는 [MC149274를 참조하세요.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**참고:** 이전에 끝점 업데이트에 HTML, XML 및 RSS를 통해 IP 또는 URL 게시를 사용한 경우 이러한 유형의 업데이트를 자동화하기 위해 새 웹 서비스로 마이그레이션해야 합니다. 자세한 내용은 끝점 범주 Microsoft 365 IP 주소 Microsoft 365 웹 서비스를 [참조하세요.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
