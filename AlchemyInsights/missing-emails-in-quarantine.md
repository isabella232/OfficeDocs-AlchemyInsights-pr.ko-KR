---
title: 격리 된 전자 메일 없음
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673720"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="fb1e6-102">격리 된 전자 메일 누락 "</span><span class="sxs-lookup"><span data-stu-id="fb1e6-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="fb1e6-103">관리자는 [이러한 메시지를 보거나 해제 하거나 삭제할](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide) 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="fb1e6-104">보안 & 준수 센터를 열려면로 이동 [https://protection.office.com](https://protection.office.com/) 합니다.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="fb1e6-105">격리 페이지를 바로 열려면로 이동 [https://protection.office.com/quarantine](https://protection.office.com/quarantine) 합니다.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="fb1e6-106">다음 값을 기준으로 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-106">You can search by the following values:</span></span>  

- <span data-ttu-id="fb1e6-107">**메시지 ID**: 메시지의 GUID(Globally Unique Identifier)입니다.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="fb1e6-108">목록에서 메시지를 선택 하는 경우 표시 되는 **세부 정보** 플라이 아웃 창에 **메시지 ID** 값이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="fb1e6-109">관리자는 [메시지 추적](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide)을 사용하여 메시지와 해당 메시지 ID 값을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="fb1e6-110">**보낸 사람 전자 메일 주소**: 보낸 사람 한 명의 전자 메일 주소입니다.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="fb1e6-111">**받는 사람 전자 메일 주소**: 받는 사람 한 명의 전자 메일 주소입니다.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="fb1e6-112">**제목**: 메시지의 전체 제목을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="fb1e6-113">검색은 대/소문자를 구분하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="fb1e6-114">검색 조건을 입력 한 후 새로 ![ 고침 단추 ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **새로** 고침을 클릭 하 여 결과를 필터링 합니다.  </span><span class="sxs-lookup"><span data-stu-id="fb1e6-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="fb1e6-115">격리에서 메시지와 파일을 보고 관리 하는 데 사용 하는 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="fb1e6-116">Delete-Get-quarantinemessage</span><span class="sxs-lookup"><span data-stu-id="fb1e6-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="fb1e6-117">Get-quarantinemessage</span><span class="sxs-lookup"><span data-stu-id="fb1e6-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="fb1e6-118">Get-quarantinemessage</span><span class="sxs-lookup"><span data-stu-id="fb1e6-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="fb1e6-119">[Preview-get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage):이 Cmdlet은 SharePoint Online, 비즈니스용 OneDrive 또는 팀에 대 한 ATP 파일이 아닌 메시지에만 해당 합니다.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="fb1e6-120">Get-quarantinemessage</span><span class="sxs-lookup"><span data-stu-id="fb1e6-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)