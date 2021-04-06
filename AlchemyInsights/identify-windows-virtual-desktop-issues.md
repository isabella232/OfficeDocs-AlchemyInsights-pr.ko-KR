---
title: Windows Virtual Desktop 문제 식별
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590297"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Windows Virtual Desktop 문제 식별

Windows Virtual Desktop 진단에서는 하나의 PowerShell cmdlet만 사용하지만 여러 선택적 매개 변수를 통해 문제를 좁히고 격리합니다. 시작하려면 다음을 수행합니다. 

1. Windows Virtual Desktop PowerShell 모듈을 다운로드하여 가져올 수 있습니다. 자세한 내용은 [Windows PowerShell용 Windows Virtual Desktop Cmdlets](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)를 참조하세요.

1. 다음 cmdlet을 실행하여 계정에 로그인합니다.
    
    예: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**참고:** PowerShell을 사용하는 모든 쿼리에는 -UserName 또는 -ActivityID 매개 변수가 포함되어야 합니다. 모니터링 기능에 대한 정보는 [진단 기능에 대한 Log Analytics](https://go.microsoft.com/fwlink/?linkid=2126847) 사용을 참조하세요.

다음 cmdlet을 실행하여 사용자가 수행한 진단 작업을 필터링합니다.

예: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

문제를 진단하기 위해 실행할 수 있는 필터 목록이 있습니다. 문제 진단에 대한 자세한 내용은 [Windows Virtual Desktop 문제 식별 및 진단](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)을 참조하세요.

일반적인 오류에 대한 자세한 내용은 [일반적인 오류 시나리오](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)를 참조하세요.
