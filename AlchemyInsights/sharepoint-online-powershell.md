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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770845"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Sharepoint Online 내에서 PowerShell 또는 스크립트 작업 자세한 내용을 보려면 아래 링크를 방문 하세요.
- [SharePoint Online 관리 셸 시작](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [다단계 인증을 사용 하 여 SPO PowerShell에 연결 (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint의 PnP (패턴 및 관행)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) 에는 SPO에 대 한 복잡 한 관리 작업을 수행할 수 있는 PowerShell 명령 라이브러리가 포함 되어 있습니다.

> [!NOTE]
> - SPO 관리 셸을 사용 하 여 연결 하는 데 문제가 있는 경우 최신 버전으로 업데이트 했는지 확인 하 고 *"import-Module Microsoft. PowerShell"* 을 사용 하 여 [모듈을 다시 가져오십시오](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) .
> - 클라이언트 쪽 개체 모델 스크립트를 실행 하려는 경우에는 로컬 컴퓨터에 [Sharepoint Online 클라이언트 구성 요소 SDK](https://www.microsoft.com/download/details.aspx?id=42038) 를 설치 해야 합니다.
> - PowerShell에서 스크립트를 실행 하는 데 문제가 있는 경우에는 PowerShell을 관리자 권한으로 실행 하 고 [실행 정책을](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)변경 하는 것을 고려해 야 합니다.