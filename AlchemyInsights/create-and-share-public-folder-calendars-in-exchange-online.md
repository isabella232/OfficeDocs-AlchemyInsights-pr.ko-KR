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
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a><span data-ttu-id="0ebe6-102">Exchange Online에서 공용 폴더 캘린더를 만들고 공유합니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-102">Create and share public folder calendars in Exchange Online</span></span>

<span data-ttu-id="0ebe6-103">Outlook 데스크톱 클라이언트에서만 공용 폴더에서 일정관리를 작성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-103">You can create a calendar in the Public folder only from the Outlook desktop client.</span></span> <span data-ttu-id="0ebe6-104">다음 단계에 따라 공용 폴더 일정관리를 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-104">Use these steps to set up public folder calendars:</span></span>

1. <span data-ttu-id="0ebe6-105">공용 폴더가 Exchange 온라인에 배포되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-105">Ensure public folders are deployed in Exchange Online.</span></span> <span data-ttu-id="0ebe6-106">자세한 내용은 [공용 폴더 사서함](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox) 만들기를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-106">For more info, see [Create a public folder mailbox](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span></span> 

2. <span data-ttu-id="0ebe6-107">공용 폴더를 만드는 데 필요한 액세스 권한이 할당되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-107">Ensure you're assigned necessary access permissions to create the public folder.</span></span> <span data-ttu-id="0ebe6-108">자세한 내용은 [Exchange 서버](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server)에 대한 공용 폴더 사용 권한을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-108">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span> 
  
3. <span data-ttu-id="0ebe6-109">Outlook 데스크톱 클라이언트에 로그인하여 공용 폴더 배포에 액세스할 수 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-109">Log in to the Outlook desktop client and ensure you can access your public folder deployment.</span></span>

    <span data-ttu-id="0ebe6-110">Outlook 데스크톱 클라이언트를 사용하여 공용 폴더에 액세스하는 데 문제가 있는 경우 [Exchange 온라인 사용자는 Outlook 또는 OWA](https://aka.ms/pfcte)를 사용하여 공용 폴더에 연결할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-110">If you're having trouble accessing public folders by using the Outlook desktop client, see [Exchange Online users can't connect to public folders by using Outlook or OWA](https://aka.ms/pfcte).</span></span>

4. <span data-ttu-id="0ebe6-111">새 공용 폴더 일정관리 유형을 작성합니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-111">Create a new public folder calendar type.</span></span>

<span data-ttu-id="0ebe6-112">공용 폴더는 기본적으로 다른 모든 사용자에게 공유됩니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-112">The public folder is shared to all other users by default.</span></span> <span data-ttu-id="0ebe6-113">공용 폴더 소유자는 Outlook 데스크톱 클라이언트에서 권한을 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-113">Owner of the public folder can change the permissions from Outlook desktop client.</span></span> <span data-ttu-id="0ebe6-114">자세한 내용은 [Exchange 서버](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server)에 대한 공용 폴더 사용 권한을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-114">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span>

<span data-ttu-id="0ebe6-115">**참고** 공용 폴더 캘린더는 조직 내에서 사용하도록 설계되었으며 인터넷에 게시할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-115">**Note** Public folder calendars are designed to be used within the organization and can't be published on the Internet.</span></span> <span data-ttu-id="0ebe6-116">캘린더를 인터넷에 게시하려는 경우 공유 편지함을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="0ebe6-116">Use a shared mailbox if your intention is to publish a calendar on the  Internet.</span></span>