---
title: 단일 사용자가 Outlook에서 추가 기능을 확인할 수 없는 경우
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 647a17bb5220d3591934c4f53cf417d42810b2c1a681bafd3e2d703abbfcbc64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050664"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>단일 사용자가 Outlook에서 추가 기능을 확인할 수 없는 경우

사용자가 올바른 AppsForOfficeEnabled 매개 변수를 갖지 않는 역할의 일부일 수 있습니다. 해당 cmdlet을 실행하여 사용자에게 올바른 역할이 연결되어 있는지 확인합니다.

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

자세한 내용은 [관리자 및 Outlook 추가 기능을 설치하고 관리할 수 있는 사용자 지정](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)을 참조하세요.
