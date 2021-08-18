---
title: 전자 메일이 검지에서 누락된 경우
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
- "5668"
- "9002625"
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329668"
---
# <a name="missing-emails-in-quarantine"></a>전자 메일이 검지에서 누락된 경우

관리자는 이러한 메시지를 [보거나 해제하거나 삭제할 수 있습니다.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

의 Microsoft 365 Defender 포털에서 Review <https://security.microsoft.com>  \> **Quarantine (으로 이동) 를 검토합니다.** 또는 **Quarantine** 페이지로 직접 이동하기 위해 를 <https://security.microsoft.com/quarantine> 사용하세요.  

사용할 수 있는 검색/필터 값에 대한 자세한 내용은 EOP에서 관리자로 [quarantined messages and files as an admin를 참조하십시오.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

메시지와 파일을 확인 및 관리하는 데 사용하는 cmdlet은 다음을 제공합니다.

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)이 cmdlet은 메시지에 대한 것이 아니라 금고, SharePoint, OneDrive 또는 Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
