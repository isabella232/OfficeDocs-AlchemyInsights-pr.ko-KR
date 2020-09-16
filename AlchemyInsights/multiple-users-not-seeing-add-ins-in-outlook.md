---
title: 여러 사용자가 Outlook 추가 기능을 확인할 수 없는 경우
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
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729877"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>여러 사용자가 Outlook 추가 기능을 확인할 수 없는 경우

Outlook 추가 기능을 테스트했지만 아무 것도 표시되지 않는 경우 첫 번째 문제 해결 단계로 **Get-OrganizationConfig** PowerShell cmdlet을 사용하여 _AppsForOfficeEnabled_ 매개 변수를 쿼리합니다. 쿼리에서 **False**값이 반환되는 경우 해당 매개 변수를 **Set-OrganizationConfig** cmdlet을 사용하여 **True**로 설정합니다. 추가 기능이 제대로 표시될 것입니다.

_AppsForOfficeEnabled_ 매개 변수를**False**로 설정하지 않는 것이 좋습니다. **False** 값은 위의 모든 관리 및 사용자 역할 설정을 재정의하고 조직의 모든 사용자가 새 앱을 활성화하지 못하도록 합니다.

자세한 내용은 [관리자 및 설치 하 고 Outlook 용 추가 기능을 관리할 수 있는 사용자 지정](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)을 참조하십시오.