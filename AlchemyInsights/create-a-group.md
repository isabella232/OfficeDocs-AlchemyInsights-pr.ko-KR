---
title: 그룹 만들기
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816362"
---
# <a name="create-a-group"></a>그룹 만들기

이 항목에서는 그룹 만들기에 대해 설명합니다.

**그룹 만들기 권한**

새 그룹을 만들 수 있는 권한을 부여해야 합니다. 전역 관리자는 Azure 포털 또는 액세스 패널에서 그룹 만들기를 사용하지 않도록 설정할 수 있습니다. 관리자가 새 그룹을 만들거나 적절한 사용 권한을 부여해야 할 수 있습니다.

**그룹 만들기 권한 관리**

1. 전역 관리자는 모든 그룹 일반(설정)에서 "사용자가 Azure Portal에서 보안 그룹을 만들 수 있습니다." 또는 "사용자가 Azure Portals에서 Office 365 그룹을 만들 수 있습니다." 옵션을 선택하여 그룹 만들기 권한(보안 관련 이유로) 또는 Azure Portal 또는 액세스 패널에서 만든 Office 365 그룹을 관리할 수 있습니다.  >  
2. Azure Active Directory P1 Premium 라이선스가 있는 경우 그룹 만들기를 제한하여 사용자 그룹을 선택할 수 있습니다.

**새 Office 365 그룹 구성원에 대한 환영 알림을 사용 안 하게 설정**

Powershell에서 **UnifiedGroupWelcomeMessageEnabled를** False로 설정하여 Office 365 그룹에 추가된 사용자에게 전송된 환영 알림을 사용하지 않도록 설정할 수 있습니다. [여기](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)에서 이 설정에 대해 자세히 알아보세요.

