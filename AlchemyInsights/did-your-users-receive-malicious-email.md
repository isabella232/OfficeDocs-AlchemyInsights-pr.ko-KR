---
title: 사용자가 악성 이메일을 받았습니까
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 608e2226c055f58ecf4f62e3c913106a6d319190ed6b317508e41514c12ba5d0
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893409"
---
# <a name="did-your-users-receive-malicious-email"></a>사용자가 악성 이메일을 받았습니까?

이제 악의적인 전자 메일을 [Microsoft 365 Defender 포털에서 제출](https://sip.security.microsoft.com/reportsubmission?viewid=admin)을 통해 Microsoft에 보고할 수 있습니다.

[관리자 제출](https://security.microsoft.com/reportsubmission?viewid=admin)에 제출된 메시지가 검색되고 세부 정보에 표시된 다음 결과가 표시됩니다.

- 전송 시 보낸 사람의 전자 메일 인증에 오류가 있는 경우입니다.
- 메시지의 평가 결과에 영향을 주거나 재정의할 수 있는 정책 조회에 대한 정보입니다.
- 메시지에 포함된 URL 또는 파일이 악의적인지 여부를 확인하는 현재 데토네이션 결과입니다.
- 채점자 피드백

재정의가 발견되면 몇 분 후에 다시 검사가 완료되어야 합니다. 전자 메일 인증에 문제가 없는 경우 또는 전송이 재정의의 영향을 받지 않았다면 성적에 대한 피드백은 최대 하루가 소요됩니다.

메시지, URL 또는 파일(차단되거나 차단되지 않은 파일)에 최종 평가 결과에 동의하지 않는 경우 다시 검색하기 위해 하루 후에 메시지를 다시 제출합니다. 메시지를 다시 제출한 후에 평가 결과가 변경될 가능성이 높습니다.

그 동안 [이 문서](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)의 지침에 따라 사용자 받은 편지함에서 악성 전자 메일을 제거할 수 있습니다.

- Office 365용 Microsoft Defender 고객은 다음을 할 수 있습니다.
  - [위협 탐색기를 사용하여 의심스러운 전자 메일 검색 및 삭제](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [안전한 링크를 사용하여 악성 URL에 액세스 차단](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links)
  - 악성 URL을 클릭하고 액세스한 사용자 추적: [피싱 URL 및 평가 결과 데이터 보기](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - 수동으로 [자동 조사 시작](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

[악성 URL 및 파일로부터 보호](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats) 지침에 따라 악성 파일 및 URL로부터 보호 받을 수 이습니다.
