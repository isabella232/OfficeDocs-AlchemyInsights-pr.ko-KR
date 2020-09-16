---
title: Outlook에서 추가 기능을 추가하는 동안 여러 사용자가 액세스 거부 오류가 발생합니다.
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
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724369"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Outlook에서 추가 기능을 추가하는 동안 여러 사용자가 액세스 거부 오류가 발생합니다.

조직에서 Outlook의 추가 기능을 설치하고 관리할 수 있는 권한을 가진 관리자를 지정할 수 있습니다. 또한 조직에서 자체 사용을 위해 추가 기능을 설치하고 관리할 수 있는 권한을 가진 사용자를 지정할 수도 있습니다.

자세한 내용은 [Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)에 대한 추가 기능을 설치하고 관리할 수 있는 관리자 및 사용자 지정을 참조합니다.

사용자에 대한 사용 권한을 성공적으로 할당했는지 확인하려면 <Role Name>을(를) 확인할 역할 이름으로 바꾸고 Exchange Online PowerShell에서 다음 명령을 실행합니다.

Get-ManagementRoleAssignment -role "<Role Name>" -GetEffectiveUsers입니다.

이 예에서는 조직에 대해 Office Store에서 추가 기능을 설치하기 위해 누구에게 권한을 할당했는지 확인하는 방법을 보여 줍니다.

PowerShell

-Role "Org Marketplace Apps" -GetEffectiveUsers

Get-ManagementRoleAssignment 결과에서 유효 사용자 열의 항목을 검토합니다.

구문과 매개 변수에 대한 자세한 내용은 [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)를 참조하십시오.
 