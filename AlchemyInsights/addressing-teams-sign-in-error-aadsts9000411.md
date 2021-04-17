---
title: Teams 로그인 오류 AADSTS9000411 해결하기
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
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821993"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="d5445-102">Teams 로그인 오류 AADSTS9000411 해결하기</span><span class="sxs-lookup"><span data-stu-id="d5445-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="d5445-103">Microsoft Teams에 로그인할 때 다음과 같은 오류가 나타날 수 있습니다. **죄송합니다. 로그인하는 데 문제가 있습니다. AADSTS9000411: 요청의 서식이 잘못 지정되었습니다. "login_hint" 매개 변수가 중복되었습니다.**</span><span class="sxs-lookup"><span data-stu-id="d5445-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="d5445-104">이 문제를 해결하려면 Microsoft Teams 클라이언트가 업데이트되어 있는지 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="d5445-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="d5445-105">클라이언트 업데이트에 대한 자세한 내용은 [Microsoft Teams 업데이트하기](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d5445-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="d5445-106">어떤 이유로 클라이언트를 업데이트할 수 없는 경우에는 클라이언트에서 로그오프하면 캐시된 데이터가 대부분 지워집니다.</span><span class="sxs-lookup"><span data-stu-id="d5445-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="d5445-107">그러나 로그오프/로그온 후에도 문제가 계속 발생하면 Teams를 종료하고 다음을 수행하여 클라이언트 캐시를 지우세요.</span><span class="sxs-lookup"><span data-stu-id="d5445-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="d5445-108">Microsoft Teams를 닫습니다.</span><span class="sxs-lookup"><span data-stu-id="d5445-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="d5445-109">%appdata%\microsoft\teams로 이동하여 모든 파일을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="d5445-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="d5445-110">Microsoft Teams를 다시 엽니다.</span><span class="sxs-lookup"><span data-stu-id="d5445-110">Reopen Microsoft Teams.</span></span>
