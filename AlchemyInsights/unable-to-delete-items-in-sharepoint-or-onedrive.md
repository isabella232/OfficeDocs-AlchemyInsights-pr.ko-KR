---
title: 사용자 계정 또는 SharePoint 항목을 삭제할 수 OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038523"
---
# <a name="unable-to-delete-items"></a>항목을 삭제할 수 없습니다.

- 보존 정책으로 인해 이 문제가 발생할 수 있습니다. 이 문제를 일으키는 각 보류를 사용하지 않도록 설정하거나 제외해야 합니다. 보존 정책 또는 보존이 제거된 후 변경이 적용되는 데 최대 24시간이 걸릴 수 있습니다. 항목에 대한 보존 정책 [설정이](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) 없는지 확인

- 사이트가 저장 용량 제한을 초과하고, 사이트 [할당량과](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) 항목을 삭제할 수 있습니다.

- 항목이 다른 사용자에게 [체크 아웃되지](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) 않은지 확인

- 마지막으로 관리자는 PowerShell [](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) 명령 라이브러리가 포함된 PnP(SharePoint 패턴 및 모범 사례)를 사용하여 스텁 항목을 강제 삭제하는 등의 복잡한 관리 작업을 수행할 수 있습니다.
- [PNP 파일 제거](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP 폴더 제거](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP 목록 항목 제거](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP 목록 제거](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP 필드 제거(열)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)