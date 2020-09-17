---
title: Exchange PowerShell과 기본 인증 중단
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: f4f0f63112d639101ea9e9d7e9a9c16a32de4cf3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782981"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell과 기본 인증 중단

기본 인증을 사용하지 않고 Exchange Online PowerShell에 연결하는 방법에 대한 최신 정보는 [여기를 참조하세요](https://aka.ms/exops-docs). PowerShell V2 모듈에서는 기본 인증을 사용하지 않습니다.

클라이언트 컴퓨터에서 기본 인증은 계속 사용하도록 설정해야 합니다.
새 PowerShell V2 모듈은 최신 인증을 사용하여 모든 REST 기반 V2 Cmdlet을 사용할 수 있도록 연결을 설정합니다. V2 cmdlet 외에도 원격 PowerShell 세션을 설정해야 하는 이전의 RPS(원격 PowerShell) Cmdlet에 액세스할 수 있습니다. Windows 컴퓨터에서 RPS 세션을 설정하려면 모듈이 최신 인증 메커니즘을 사용하여 서비스에서 인증을 받는 경우에도, 클라이언트 컴퓨터에서 WinRM BasicAuth를 사용하도록 설정해야 합니다. WinRM 기본 인증 파이프라인은 최신 인증 토큰을 전송하는 데 사용됩니다. 클라이언트 컴퓨터에서 WinRM 기본 인증을 사용하지 않도록 설정한 경우에는 새 V2 cmdlet이 계속 작동하지만 이전 RPS cmdlet은 작동하지 않습니다.
