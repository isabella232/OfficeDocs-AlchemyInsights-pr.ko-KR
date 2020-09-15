---
title: Outlook에 추가 기능을 추가 하는 동안 한 명의 사용자에게 액세스 거부 오류 발생
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 355f37386e0a498185e195c1d715386785d0b54b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673287"
---
# <a name="one-user-gets-access-denied-error-while-adding-add-ins-in-outlook"></a>Outlook에 추가 기능을 추가 하는 동안 한 명의 사용자에게 액세스 거부 오류 발생

권한을 찾는 PowerShell 사용자

ManagementRoleAssignment-얻기 -RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -Delegating $false | 포맷-표 -자동 역할,RoleAssigneeName,RoleAssigneeType