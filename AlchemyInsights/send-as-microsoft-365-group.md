---
title: Microsoft 365 그룹으로 보내기
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 204b2c1777f76f11663b2735b784cbb56f1f1aba891628fb46ef37b501c9ff85
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086134"
---
# <a name="send-as-microsoft-365-group"></a>Microsoft 365 그룹으로 보내기

특정 사용자가 Microsoft 365 그룹으로 메시지를 보낼 수 있도록 다른 사람 이름으로 보내기 권한을 할당할 수 있습니다.  

1. Exchange Online PowerShell에 연결합니다.  

2. 다음 명령을 실행합니다.  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

자세한 내용은 [그룹을 사용하여 다른 이름으로 보내거나 그룹을 대신하여 보내기](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)를 참조 하세요.