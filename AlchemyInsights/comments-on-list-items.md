---
title: 목록 항목에 대한 설명
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995493"
---
# <a name="comments-on-list-items"></a>목록 항목에 대한 설명

사용자는 목록 항목의 모든 설명을 보고 항목과 관련된 설명이나 활동을 표시하는 보기 간에 필터링할 수 있습니다.

사용자는 설명을 추가하고 삭제하기 전에 다음에 유의해야 합니다.

- 설명은 설명에 있는 사용 권한 설정을 SharePoint.
- 작업 목록과 같은 최신 사용자 인터페이스에 표시하도록 아직 만들어지지 않은 클래식 목록에는 이 주석 기능이 없습니다.
- 이 릴리스에서는 Teams 목록에 대한 설명을 사용할 수 없습니다.
- 설명은 검색에서 인덱싱되지 않습니다.

관리자는 **Set-SPOTenant** PowerShell cmdlet에서 **CommentsOnListItemsDisabled** 매개 변수를 변경하여 조직 수준에서 이 기능을 사용하지 않도록 설정할 수 있습니다.

현재 사이트 또는 목록 수준에서 주석을 사용하지 않도록 설정할 수 없습니다. 2021년 1분기 이후 업데이트에서 이러한 컨트롤을 사용할 수 있을 것입니다.
