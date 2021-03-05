---
title: Microsoft 365의 감사
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464893"
---
# <a name="auditing-in-microsoft-365"></a><span data-ttu-id="11bf6-102">Microsoft 365의 감사</span><span class="sxs-lookup"><span data-stu-id="11bf6-102">Auditing in Microsoft 365</span></span>

<span data-ttu-id="11bf6-103">다음은 Microsoft 365의 감사에 대해 알아야 할 몇 가지 사항입니다.</span><span class="sxs-lookup"><span data-stu-id="11bf6-103">Here are a few things you should know about auditing in Microsoft 365:</span></span>

1. <span data-ttu-id="11bf6-104">Exchange 관리자 활동은 기본적으로 감사됩니다.</span><span class="sxs-lookup"><span data-stu-id="11bf6-104">Exchange admin activities are audited by default.</span></span>
1. <span data-ttu-id="11bf6-105">기본적으로 모든 사용자에 대해 사서함 감사를 켜는 중입니다.</span><span class="sxs-lookup"><span data-stu-id="11bf6-105">We're in the process of turning on mailbox auditing by default for all users.</span></span> <span data-ttu-id="11bf6-106">이에 대한 자세한 내용을 보려면 여기를 [클릭하세요.](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171)</span><span class="sxs-lookup"><span data-stu-id="11bf6-106">To read more about this, click [here](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span></span> <span data-ttu-id="11bf6-107">그 때까지 한 사람 또는 전체 조직에 대해 수동으로 사용하도록 설정하려면 아래 사서함 감사 켜기 단추를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="11bf6-107">Until then, if you want instructions to manually enable it for one person or an entire organization, choose the Turn on mailbox auditing button below.</span></span>
1. <span data-ttu-id="11bf6-108">Microsoft 365 그룹 사서함 및 공용 폴더 사서함은 감사 로깅을 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="11bf6-108">Microsoft 365 Groups mailboxes and Public Folder mailboxes do not support audit logging.</span></span>
1. <span data-ttu-id="11bf6-109">SharePoint/OneDrive의 경우 감사를 사용하도록 설정하는 데 추가 구성이 필요하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="11bf6-109">For SharePoint/OneDrive, there is no additional configuration required to enabled auditing.</span></span> <span data-ttu-id="11bf6-110">감사할 활동은 다음을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="11bf6-110">To learn what activities are audited, see:</span></span>
    1. [<span data-ttu-id="11bf6-111">파일 활동</span><span class="sxs-lookup"><span data-stu-id="11bf6-111">File activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [<span data-ttu-id="11bf6-112">폴더 활동</span><span class="sxs-lookup"><span data-stu-id="11bf6-112">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. <span data-ttu-id="11bf6-113">[공유 및 액세스 활동](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span><span class="sxs-lookup"><span data-stu-id="11bf6-113">[Sharing and Access activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span></span>
1. <span data-ttu-id="11bf6-114">서비스로 감사된 모든 활동 목록은 감사된 활동을 [참조하세요.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)</span><span class="sxs-lookup"><span data-stu-id="11bf6-114">For a list of all audited activities by service, see [Audited activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>
