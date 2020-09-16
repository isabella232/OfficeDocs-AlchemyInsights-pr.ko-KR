---
title: Microsoft를 가리키도록 도메인 이름 서버 업데이트
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734917"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Microsoft를 가리키도록 도메인 이름 서버 업데이트

참고: 네임 서버 변경 사항이 전파되는 데 최대 48 시간이 걸릴 수 있습니다.
  
Microsoft에서 도메인을 설정 하려면 등록자에서 이름 서버를 업데이트 해야 합니다. 도메인 등록 기관에서 이름 서버 레코드를 만들거나 편집합니다.
  
1. 도메인 등록 기관 웹 사이트에서 이름 서버를 편집하는 곳을 찾습니다.

2. 아래의 값을 갖는 2개의 이름 서버 레코드를 만들거나 편집합니다.

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. 변경 내용을 저장합니다.

또한이 문서에서 [이름 서버를 변경 하 여 도메인 등록 기관으로 Microsoft 365을 설정 하](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar) 는 방법에 대 한 자세한 지침을 확인할 수 있습니다.
  