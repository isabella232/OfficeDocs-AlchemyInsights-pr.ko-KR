---
title: Microsoft 이름 서버에서 자체 DNS 레코드 관리로 다시 변경
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/22/2021
ms.locfileid: "59481869"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Microsoft 이름 서버에서 자체 DNS 레코드 관리로 다시 변경

이전에 NS 레코드가 Microsoft(ns1.bdm.microsoftonline.com)를 가리키도록 변경했지만 이제 자체 DNS 레코드를 관리하기로 결정했습니다.

도메인 등록 대행자의 웹사이트에서 이름 서버를 등록 기관 또는 이전 설정으로 다시 변경하세요. DNS에 익숙하지 않은 경우 도메인 등록 기관의 지원에 문의하세요. 이름 서버 변경 사항이 적용되는 데 최대 48시간이 소요될 수 있습니다. 

1. Microsoft 365 관리 포털에서 **설정** > [**도메인**](https://admin.microsoft.com/Adminportal/Home#/Domains)으로 이동하고 도메인 옆의 확인란을 선택한 다음 **DNS 관리** 를 선택합니다. 

2. 마법사에서 **자체 DNS 레코드 추가** 를 선택하고 마법사를 완료합니다. 이렇게 하면 DNS 관리 방식이 변경되고 선택한 서비스를 지원하는 데 필요한 사용자 지정 DNS 레코드를 추가할 수 있습니다.

또는 이름 서버 레코드를 Microsoft로 변경하고 웹사이트가 있는 경우 이름 서버를 다시 변경하는 대신 웹사이트에 대한 DNS 레코드를 추가할 수 있습니다. 자세한 내용은 [현재 호스팅 제공업체에서 웹사이트를 유지하도록 DNS 레코드 업데이트](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)를 참조하세요.


