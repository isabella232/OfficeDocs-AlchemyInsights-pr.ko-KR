---
title: 공유 링크에서 다운로드 차단
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
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685748"
---
# <a name="block-download-on-sharing-links"></a>공유 링크에서 다운로드 차단

**다운로드 차단**은 Office 문서의 **보기 전용 링크**에만 사용 가능합니다. 해당 옵션을 선택하면, 링크를 통한 파일 액세스가 허용된 사용자에게 더 이상 파일 다운로드, 프린트 또는 복사 옵션이 보이지 않게 됩니다.

관리자는 `BlockDownloadLinksFileType`[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) 또는 [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets에서 설정을 변경하여 “다운로드 차단” 설정이 Office 파일에서만 보이도록 할지 여부를 제어할 수 있습니다.
