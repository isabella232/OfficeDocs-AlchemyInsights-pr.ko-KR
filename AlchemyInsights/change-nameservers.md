---
title: 이름 서버 변경
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 3f39bfc585e8b805424cb7ccac76f81e1b2bfda9dcd1367361fec6a668c545bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017786"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Microsoft를 가리키도록 도메인 이름 서버 업데이트

참고: 네임 서버 변경 사항이 전파되는 데 최대 48 시간이 걸릴 수 있습니다.
  
Microsoft 365에서 도메인을 설정하려면 등록 기관의 이름 서버를 업데이트해야 합니다. 도메인 등록 기관에서 이름 서버 레코드를 만들거나 편집합니다.
  
1. 도메인 등록 기관 웹 사이트에서 이름 서버를 편집하는 곳을 찾습니다.
  
2. 아래의 값을 갖는 2개의 이름 서버 레코드를 만들거나 편집합니다.

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. 변경 내용을 저장합니다.

다음 문서에서도 자세한 방법을 확인할 수 있습니다. [도메인 등록 기관에서 이름 서버 변경](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  