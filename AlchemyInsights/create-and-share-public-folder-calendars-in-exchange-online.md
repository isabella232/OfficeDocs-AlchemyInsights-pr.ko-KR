---
title: Exchange Online에서 공용 폴더 캘린더를 만들고 공유합니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: d8b28d373db21da42b90aeef75139affd802a5d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712645"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a>Exchange Online에서 공용 폴더 캘린더를 만들고 공유합니다.

Outlook 데스크톱 클라이언트에서만 공용 폴더에서 일정관리를 작성할 수 있습니다. 다음 단계에 따라 공용 폴더 일정관리를 설정할 수 있습니다.

1. 공용 폴더가 Exchange 온라인에 배포되었는지 확인합니다. 자세한 내용은 [공용 폴더 사서함](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox) 만들기를 참조합니다. 

2. 공용 폴더를 만드는 데 필요한 액세스 권한이 할당되었는지 확인합니다. 자세한 내용은 [Exchange 서버](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server)에 대한 공용 폴더 사용 권한을 참조합니다. 
  
3. Outlook 데스크톱 클라이언트에 로그인하여 공용 폴더 배포에 액세스할 수 있는지 확인합니다.

    Outlook 데스크톱 클라이언트를 사용하여 공용 폴더에 액세스하는 데 문제가 있는 경우 [Exchange 온라인 사용자는 Outlook 또는 OWA](https://aka.ms/pfcte)를 사용하여 공용 폴더에 연결할 수 없습니다.

4. 새 공용 폴더 일정관리 유형을 작성합니다.

공용 폴더는 기본적으로 다른 모든 사용자에게 공유됩니다. 공용 폴더 소유자는 Outlook 데스크톱 클라이언트에서 권한을 변경할 수 있습니다. 자세한 내용은 [Exchange 서버](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server)에 대한 공용 폴더 사용 권한을 참조합니다.

**참고** 공용 폴더 캘린더는 조직 내에서 사용하도록 설계되었으며 인터넷에 게시할 수 없습니다. 캘린더를 인터넷에 게시하려는 경우 공유 편지함을 사용합니다.