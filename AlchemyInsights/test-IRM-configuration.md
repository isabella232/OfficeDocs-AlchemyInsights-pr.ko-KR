---
title: 새 OME 기능에 대한 IRM 구성 테스트
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: d084caabfbcfdd92d6b90554c9e2bef5f571a0227827332a5fb3d710d7bc4836
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899702"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>새 OME 기능에 대한 IRM 구성 테스트

Microsoft 365 테넌트가 새 OME 기능을 사용하도록 구성되어 있는지 확인하려면 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online-powershell)에 연결된 상태에서 다음 cmdlet을 실행합니다.


1. `Get-IRMConfiguration`을(를) 실행하여 테넌트의 IRM 구성을 확인합니다. 이러한 값이 **true** 로 설정되었는지 확인합니다.
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. 도메인, 발신자 주소 및 수신자를 사용하여 `Test-IRMConfiguration`을(를) 실행합니다. 테스트가 통과되지 않으면 IRM 구성을 조사합니다.

IRM 구성을 확인하는 방법에 대한 자세한 내용은 [Exchange Online PowerShell의 새 OME 구성 확인](https://docs.microsoft.com/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)을 참조하세요.