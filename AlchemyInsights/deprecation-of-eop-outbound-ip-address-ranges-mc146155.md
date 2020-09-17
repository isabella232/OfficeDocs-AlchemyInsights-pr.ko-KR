---
title: 1065 EOP 아웃 바운드 IP 주소 rangesMC146155의 중단
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
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806801"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP 아웃 바운드 IP 주소 범위 중단

조직에서 잠재적인 문제를 감지 했으며 (이 경우, 2018에서 수정 하지 않은 경우) 온-프레미스 또는 외부 대상으로 메일 흐름이 중단 될 수 있습니다. 이전에는 IP 주소 범위 관리를 단순화 하기 위해 EOP (Exchange Online Protection) IP 주소 범위가 Microsoft 365 외부에서 전자 메일을 보내고 받는 데 사용 됩니다. 이 분석은 메일 흐름 커넥터에 구성한 하나 이상의 외부 전자 메일 원본 또는 대상이 [여기](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)에 표시 된 IP 주소 범위 로부터의 연결을 수락 하지 않음을 의미 합니다.

이 원본 및 대상에서 게시 된 모든 [EOP IP 주소](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)간의 연결을 허용 하도록 하려면 10 월 26th 이전에 역할을 수행 합니다.

이 변경 내용에 대 한 자세한 내용은 Message Center 게시물 [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)또는 [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)를 참조 하십시오.

**참고**: 끝점 업데이트를 위해 HTML, XML 및 RSS를 통해 이전에 IP 또는 URL 게시를 사용한 경우 이러한 유형의 업데이트를 자동화 하기 위해 새 웹 서비스로 마이그레이션해야 합니다. 자세한 내용은 [microsoft 365 끝점 범주 및 microsoft 365 IP 주소 및 URL 웹 서비스](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)를 참조 하세요.
