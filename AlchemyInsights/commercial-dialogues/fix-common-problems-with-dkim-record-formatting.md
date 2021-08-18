---
title: DKIM 레코드 서식의 일반적인 문제 해결
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323996"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>DKIM 레코드 서식의 일반적인 문제 해결

대부분의 DKIM 설정 문제는 잘못된 DNS 레코드와 관련이 있습니다.

DKIM 설정 문제를 해결하려면 DKIM CNAME 레코드(TXT 레코드 아님)의 서식이 올바르게 지정되어 있는지 확인합니다. 자세한 내용은 에서 [DKIM을](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)수동으로 설정하기 위해 필요한 Office 365.

일반적으로 DNS 레코드에 대한 도움이 필요한 경우 [DNS](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)호스팅 공급자에서 DNS 레코드 만들기를 Office 365.

**참고:** 도메인의 DNS 호스팅 서비스에서 DKIM DNS 레코드를 만들거나 업데이트한 후 DNS 레코드가 전파될 때까지 기다려야 합니다.
