---
title: 공용 폴더 숨기기
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 66c76947d553c32475ebe7a11e69246b5b3a2882bb3d022873d85b93b3e87887
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945748"
---
# <a name="hide-public-folders"></a>공용 폴더 숨기기

**전체 공용 폴더 트리를 숨기려면**:

[이](https://aka.ms/ControlPF) 문서의 단계를 사용하여 선택적 또는 전체 사용자로부터 전체 공용 폴더 트리를 숨기세요.

**특정 공용 폴더를 숨기려면**:

1. 공용 폴더에 액세스해야 하는 사용자에 대한 사용 권한 추가

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. **사용 권한** 목록에서 사용자 **기본값** 을 제거합니다.

    `Remove-PublicFolderClientPermission \test1 -User Default`
