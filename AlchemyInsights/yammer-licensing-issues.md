---
title: Yammer 라이선스 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989736"
---
# <a name="yammer-licensing-issues"></a>Yammer 라이선스 문제

Yammer Enterprise 서비스를 사용하려는 모든 사용자는 라이선스를 보유하고 있어야 하지만 기본적으로 Yammer 서비스에 액세스 하는데 라이선스가 필요하지는 않습니다. 관리자가 Yammer 라이선스가 없는 Microsoft 365 사용자를 차단하도록 설정하면 Yammer Enterprise 라이선스를 할당하지 않는 사용자는 Yammer 서비스에 액세스 할 수 없습니다. 자세한 내용은 [Office 365에서 Yammer 사용자 라이선스 관리](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)를 참조하세요. 

라이선스가 사용자에게서 삭제되면 Yammer 타일은 더 이상 보이지 않고 다른 서비스는 기능을 숨기기 위해 라이선스 삭제를 사용할 수 있습니다. 경우에 따라 기능을 계속 사용할 수 있지만 운영하기 위해서는 라이선스 할당이 필요합니다.  

**라이선스가 업데이트 되지 않습니다**  

가끔 사용자에게 라이선스가 할당 되었지만 Yammer에 액세스 하지 못할 수 있습니다. 대량 라이선스가 할당 되는 경우 지연이 발생 할 수 있습니다. 시스템이 비동기적으로 실행되므로 Azure AD에서 라이선스가 변경되는 것과 동일한 순서로 Yammer 사용자 업데이트가 되지 않을 수 있습니다. 라이선스 동기화 문제를 지원에 보고하기 전에 24시간을 기다립니다.  

**대량 라이선스 할당**  

라이선스는 관리 센터 또는 PowerShell 스크립트를 통해 할당할 수 있습니다. 자세한 내용은 [사용자에게 라이선스 할당](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) 및 [Office 365 PowerShell 사용자 계정으로 라이선스 할당](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)을 참조하세요. 

Microsoft 지원에서는 스크립트 만들기 지원을 제공하지 않지만 Yammer 라이선스 할당 관련 문서를 사용할 수 있습니다. 자세한 내용은 [Windows PowerShell을 사용하여 Yammer 라이선스 관리](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)를 참조하세요.