---
title: 차트에서 다양한 수의 레코드를 표로 표시
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 68ba6caf602a5cf60e2c96c80703f19dd07c3b6430c2a66f40fea4a2f3d06e75
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950086"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>차트에서 다양한 수의 레코드를 표로 표시

**증상**

대시보드 페이지의 차트에서 차트 "…"를 클릭하고 "레코드 보기"를 클릭하면 표 페이지로 이동하여 모든 레코드를 볼 수 있습니다. 가끔 레코드 수가 변경되는 경우도 있습니다.

**원인**

이는 원본 대시보드 페이지의 차트와 표 홈 페이지의 차트 간에 차이가 있기 때문입니다.  

**솔루션**

1. 원본 페이지의 보기와 표의 보기가 서로 다른지 확인합니다.
2. 원본 페이지의 보기에 맞게 표의 보기를 변경합니다.
3. 올바른 보기를 찾을 수 없는 경우 일반적으로 이는 앱 디자이너에서 보기를 사용하도록 설정되어 있지 않음을 나타냅니다.
4. 특정 앱의 앱 디자이너로 이동하여 엔터티와 해당 보기를 선택한 후 사용하도록 설정하고, 저장하고, 게시하고, 닫으려는 보기를 표시합니다.
5. 페이지를 새로 고칩니다.