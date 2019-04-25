---
title: 감사 로그에서 IP 주소 및 클라이언트 식별
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909363"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>감사 로그에서 IP 주소 및 클라이언트 식별

사용자 또는 관리자가 수행한 활동에 해당 하는 IP 주소가 감사 로그에 표시 됩니다. 클라이언트 정보도 기록 됩니다. 이러한 정보를 식별 하는 단계는 다음과 같습니다.

1. [Office 365 Security & 준수 센터](https://protection.office.com/) 에 로그인 합니다.

2. **검색 및 조사** 를 클릭 하 고 **감사 로그 검색**을 선택 합니다.

   특정 활동에 관심이 있는 경우 **작업** 목록에서 선택 합니다. 그렇지 않으면 선택한 사용자에 대 한 모든 작업이 반환 됩니다 (기본 설정).

   **참고**: 특정 활동은 **활동** 메뉴에서 사용 하지 못할 수 있습니다. 그러나 **모든 작업에 대 한 결과 표시** (기본 설정)가 선택 되어 있으면 이러한 감사 항목이 반환 됩니다.

3. **사용자** 필드에서 사용자 이름을 지정 하 고 활동에 적합 한 날짜 범위를 선택한 다음 **검색**을 클릭 합니다.

결과 창에서 해당 활동의 IP 주소를 확인할 수 있습니다. 감사 레코드를 선택 하 여 **세부** 정보 플라이 아웃 (예: 클라이언트, 작업을 수행한 사용자)에서 자세한 내용을 확인 합니다.

자세한 내용은 [손상 된 계정에 액세스 하는 데 사용 되는 컴퓨터의 IP 주소 찾기를](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)참조 하십시오.