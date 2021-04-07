---
title: 삭제된 Microsoft 365 그룹 복원
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597449"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>삭제된 Microsoft 365 그룹 복원

삭제 후 30일 이내에 삭제된 Microsoft 365 그룹 또는 Microsoft Teams를 복원할 수 있습니다.

1. [Microsoft 365](https://aka.ms/RestoreDeletedGroup) 관리 센터로 이동하여 로그인하고 삭제된 그룹 및 팀을 나열합니다.

    **참고:** 테넌트 관리자 또는 그룹 관리자 역할에 할당된 계정을 사용하여 로그인합니다.

1. 복원할 삭제된 Microsoft 365 그룹/Teams를 선택하고 그룹 **복원을 클릭합니다.**

    충돌하는 SMTP 주소로 인해 그룹을 복원할 수 없는 경우 다음 명령을 사용하여 충돌을 일으키는 개체를 찾고 SMTP 주소를 제거합니다.

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **참고:** 경우에 따라 그룹 및 모든 데이터를 복원하는 데 24시간이 걸릴 수 있습니다.

    자세한 내용을 보거나 PowerShell을 사용하여 그룹을 복원하는 방법에 대한 자세한 내용은 삭제된 [Microsoft 365 그룹 복원을 참조하세요.](https://go.microsoft.com/fwlink/?linkid=867802)