---
title: 감사 로그의 받은 편지함 규칙 활동 식별
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779057"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="3724d-102">감사 로그의 받은 편지함 규칙 활동 식별</span><span class="sxs-lookup"><span data-stu-id="3724d-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="3724d-103">Microsoft 365 보안 & 준수 센터에서 감사 로그 검색을 사용 하 여 받은 편지함 규칙을 만들고, 수정 하 고, 삭제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3724d-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="3724d-104">[Microsoft 365 보안 & 준수 센터](https://protection.office.com/)에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="3724d-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="3724d-105">**검색**  >  **감사 로그 검색** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="3724d-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="3724d-106">**시작 날짜** 및 **끝 날짜** 필드에서 날짜 범위를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3724d-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="3724d-107">**Exchange 사서함 활동**에서 **작업** 필드가 **disable-inboxrule 만들기/수정/사용/사용 안 함 받은 편지함 규칙**으로 설정 되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="3724d-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="3724d-108">**검색**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="3724d-108">Click **Search**.</span></span>

<span data-ttu-id="3724d-109">결과에서 감사 레코드를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="3724d-109">In the results, select an audit record.</span></span> <span data-ttu-id="3724d-110">세부 정보 플라이 아웃에서 **추가 정보**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="3724d-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="3724d-111">받은 편지함 규칙 설정에 대 한 정보는 **매개 변수** 필드에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3724d-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="3724d-112">자세한 내용은 [사용자가 받은 편지함 규칙을 만들었는지 확인](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) 을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="3724d-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
