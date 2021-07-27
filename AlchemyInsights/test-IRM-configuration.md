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
ms.openlocfilehash: 28267a4cd0aa139467327385b8e85fed1675cf19
ms.sourcegitcommit: 86c95d3f0f268e500b3732243ca85a650b2e7b8f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53533006"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>새 OME 기능에 대한 IRM 구성 테스트

Microsoft 365 테넌트가 새 OME 기능을 사용하도록 구성되어 있는지 확인하려면 [Exchange Online PowerShell](/powershell/exchange/exchange-online-powershell)에 연결된 상태에서 다음 cmdlet을 실행합니다.


1. `Get-IRMConfiguration`을(를) 실행하여 테넌트의 IRM 구성을 확인합니다. 이러한 값이 **true** 로 설정되었는지 확인합니다.
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. 도메인, 발신자 주소 및 수신자를 사용하여 `Test-IRMConfiguration`을(를) 실행합니다. 테스트가 통과되지 않으면 IRM 구성을 조사합니다.

IRM 구성을 확인하는 방법에 대한 자세한 내용은 [Exchange Online PowerShell의 새 OME 구성 확인](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)을 참조하세요.