---
title: 목록 항목에 대 한 설명
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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947506"
---
# <a name="comments-on-list-items"></a>목록 항목에 대 한 설명

사용자가 목록 항목에 대 한 설명을 추가 및 삭제할 수 있습니다. 사용자는 목록 항목에 대 한 모든 의견을 보고 항목과 관련 된 메모 또는 활동을 표시 하는 보기를 필터링 할 수 있습니다.

**타이밍** :

**대상** 지정 된 릴리스: 중간-10 시에 점진적으로 롤업 되며, 11 월 중반에 완료 될 예정입니다.

**표준 릴리스** : 12 월 이전에 점진적으로 롤오버 하 여 완료 될 예정입니다.

**롤아웃** : 전체 조직에 대 한 대상 지정 릴리스

사용자는 설명을 추가 및 삭제 하기 전에 다음을 기록해 야 합니다.

- 설명은 SharePoint의 고유한 사용 권한 설정에 따릅니다.
- 아직 최신 사용자 인터페이스에 표시 되도록 작성 되지 않은 클래식 목록 (작업 목록 등)은이 주석 달기 기능을 제공 하지 않습니다.
- 이번 릴리스에서는 팀의 목록에 대해 주석을 사용할 수 없습니다.
- 검색을 통해 메모가 인덱싱되지 않습니다.

관리자는 **Set-spotenant** PowerShell Cmdlet에서 **CommentsOnListItemsDisabled** 매개 변수를 변경 하 여 조직 수준에서이 기능을 사용 하지 않도록 설정할 수 있습니다.

현재 사이트 또는 목록 수준에서 주석을 사용 하지 않도록 설정할 수는 없습니다. 이번에는 1/4 분기 2021에 해당 하는 최신 업데이트에서 해당 컨트롤을 사용할 수 있습니다.
