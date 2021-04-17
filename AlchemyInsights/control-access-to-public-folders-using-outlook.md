---
title: Outlook을 사용하여 공용 폴더에 대한 액세스 제어하기
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816746"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Outlook을 사용하여 공용 폴더에 대한 액세스 제어하기

Outlook을 사용하여 공용 폴더에 액세스할 수 있는 사용자를 제어하려면:

1. `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` 사용

$true: Outlook의 공용 폴더에 대한 사용자 액세스 허용  
$false: Outlook의 공용 폴더에 대한 사용자 액세스 차단 이 값은 기본값입니다.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

참고: 이 절차는 Windows 클라이언트용 Outlook 데스크톱과의 연결만 제어합니다. 사용자는 OWA 또는 Mac용 Outlook을 사용하여 공용 폴더에 계속 액세스할 수 있습니다.

자세한 내용은 [Outlook의 공용 폴더에 대한 제어된 연결](https://aka.ms/controlpf)을 참조하세요.
