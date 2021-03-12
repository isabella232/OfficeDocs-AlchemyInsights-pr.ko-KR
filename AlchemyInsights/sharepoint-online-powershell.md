---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709076"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Sharepoint Online 내에서 PowerShell 또는 스크립트를 사용하나요? 자세한 내용은 아래 링크를 방문하세요.
- [SharePoint Online 관리 셸 시작](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [MFA(다단계 인증)를 사용하여 SPO PowerShell에 연결](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint PnP(패턴 및](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) 모범 사례)에는 SPO에 대해 복잡한 관리 작업을 수행할 수 있는 PowerShell 명령 라이브러리가 포함되어 있습니다.

> [!NOTE]
> - SPO 관리 셸에 연결하는 데 문제가 있는 경우 최신 버전으로 업데이트한 [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) 후 *"Import-Module Microsoft.Online.SharePoint.PowerShell"을* 사용하여 모듈을 다시 가져와야 합니다.
> - 클라이언트 쪽 개체 모델 스크립트를 실행하려는 경우 로컬 컴퓨터에 Sharepoint Online 클라이언트 구성 요소 [SDK를](https://www.microsoft.com/download/details.aspx?id=42038) 설치해야 합니다.
> - PowerShell에서 스크립트를 실행하는 데 문제가 있는 경우 PowerShell을 관리자 권한으로 실행하고 실행 정책을 변경하는 [것을 고려할 수 있습니다.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)