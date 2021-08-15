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
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026228"
---
# <a name="missing-emails-in-quarantine"></a>전자 메일이 없는 경우"

관리자는 이러한 메시지를 [보거나 해제하거나 삭제할 수 있습니다.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

보안 및 준수 & 열기 위해 로 이동 [https://protection.office.com](https://protection.office.com/) 합니다. Quarantine 페이지를 직접 열기 위해 로 [https://protection.office.com/quarantine](https://protection.office.com/quarantine) 이동합니다.  

다음 값을 기준으로 검색할 수 있습니다.  

- **메시지 ID**: 메시지의 GUID(Globally Unique Identifier)입니다. 목록에서 메시지를 선택하면 메시지  **ID**  값이 나타나는 세부 정보  **플라이아웃**  창에 나타납니다. 관리자는 [메시지 추적](/microsoft-365/security/office-365-security/message-trace-scc)을 사용하여 메시지와 해당 메시지 ID 값을 찾을 수 있습니다.
- **보낸 사람 전자 메일 주소**: 보낸 사람 한 명의 전자 메일 주소입니다.
- **받는 사람 전자 메일 주소**: 받는 사람 한 명의 전자 메일 주소입니다.
- **제목**: 메시지의 전체 제목을 사용합니다. 검색은 대/소문자를 구분하지 않습니다.

검색 조건을 입력한 후 ![새로 고침 단추](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **새로 고침** 을 클릭하여 결과를 필터링합니다.

메시지와 파일을 확인 및 관리하는 데 사용하는 cmdlet은 다음을 제공합니다.
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)이 cmdlet은 Microsoft Defender에서 Office 365 Online, 비즈니스용 OneDrive SharePoint 또는 앱용 맬웨어 파일이 아니라 메시지에만 사용할 수 Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)