---
title: DNS 레코드를 업데이트하여 현재 호스팅 공급자에 웹 사이트 유지
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815791"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS 레코드를 업데이트하여 현재 호스팅 공급자에 웹 사이트 유지

1. Microsoft 365 관리 센터에서 **설치**  >  [도메인](https://admin.microsoft.com/Adminportal#/Domains) 페이지로 이동 하 여 도메인 목록에서 웹 사이트에 사용 중인 도메인을 선택 합니다.

2. **+ 새 사용자 지정 레코드** 를 선택하고 다음을 입력합니다.

  - **DNS 유형** 에 대해 다음을 입력합니다. **A(주소)**

  - **호스트 이름 또는 별칭** 에는 **@** 을 입력합니다.

  - **IP 주소** 에는 현재 호스팅되는 웹 사이트의 고정 IP 주소를 입력합니다(예: 172.16.140.1).

    이 IP 주소는  *동적*  IP 주소가 아니라 웹 사이트의  *고정*  IP 주소여야 합니다. 웹 사이트가 호스트되는 사이트에서 공개 웹 사이트의 고정 IP 주소를 가져올 수 있는지 확인합니다.

3. **저장** 을 선택합니다.

추가로, 고객이 쉽게 사용자의 웹 사이트를 찾을 수 있도록 CNAME 레코드를 만들 수 있습니다.
  
1. **+ 새 사용자 지정 레코드** 를 선택하고 다음을 입력합니다.

  - **DNS 유형** 에 대해 다음을 입력합니다. **CNAME(별칭)**

  - **호스트 이름 또는 별칭** 에는 **www** 를 입력합니다.

  - **대상 주소** 에 웹 사이트의 FQDN(정규화된 도메인 이름)을 contoso.com과 같이 입력합니다.

2. **저장**을 선택합니다.
