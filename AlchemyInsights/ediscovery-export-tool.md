---
title: eDiscovery 내보내기
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101308"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>eDiscovery 내보내기 도구를 설치하거나 실행할 수 없는 경우

eDiscovery 내보내기 도구를 설치하거나 실행하여 검색 결과를 다운로드할 수 없는 경우 다음을 검사합니다.
  
- 사용하는 컴퓨터가 다음의 선행 요구 사항을 충족합니다.

  - 32비트 및 64비트 버전의 Windows 7 이상 버전

  - Microsoft .NET Framework 4.7

  - 지원 브라우저:

  - Microsoft Edge

    또는

  - Internet Explorer 10 이상 버전

    Google Chrome 및 Mozilla Firefox와 같은 기타 브라우저는 지원되지 않습니다.

- 조직은 .blob.core.windows.net Azure의 끝점에 연결할 수 있습니다(와일드카드는 내보내기 작업의 고유 **\* 식별자를** 나타임).

- 보안 및 준수 센터에서 내보내기 Microsoft 365 &amp; 할당됩니다. 기본적으로 이 역할은 eDiscovery 관리자 역할 그룹에만 할당됩니다. [eDiscovery 사용 권한 할당을 참조합니다.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

자세한 내용은 콘텐츠 검색 결과 [내보내기 를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

100K 사서함을 내보낼 경우 내보내기 결과를 다운로드하려면 다음 Powershell을 사용하여  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)사서함에서 결과 내보내기 를 다운로드해야 합니다.