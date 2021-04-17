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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831740"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="f2055-102">전자 메일이 없는 경우"</span><span class="sxs-lookup"><span data-stu-id="f2055-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="f2055-103">관리자는 이러한 메시지를 [보거나 해제하거나 삭제할 수 있습니다.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="f2055-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="f2055-104">보안 및 준수 & 열기 위해 로 이동 [https://protection.office.com](https://protection.office.com/) 합니다.</span><span class="sxs-lookup"><span data-stu-id="f2055-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="f2055-105">Quarantine 페이지를 직접 열기 위해 로 [https://protection.office.com/quarantine](https://protection.office.com/quarantine) 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="f2055-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="f2055-106">다음 값을 기준으로 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f2055-106">You can search by the following values:</span></span>  

- <span data-ttu-id="f2055-107">**메시지 ID**: 메시지의 GUID(Globally Unique Identifier)입니다.</span><span class="sxs-lookup"><span data-stu-id="f2055-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="f2055-108">목록에서 메시지를 선택하면 메시지  **ID**  값이 나타나는 세부 정보  **플라이아웃**  창에 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="f2055-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="f2055-109">관리자는 [메시지 추적](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide)을 사용하여 메시지와 해당 메시지 ID 값을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f2055-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="f2055-110">**보낸 사람 전자 메일 주소**: 보낸 사람 한 명의 전자 메일 주소입니다.</span><span class="sxs-lookup"><span data-stu-id="f2055-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="f2055-111">**받는 사람 전자 메일 주소**: 받는 사람 한 명의 전자 메일 주소입니다.</span><span class="sxs-lookup"><span data-stu-id="f2055-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="f2055-112">**제목**: 메시지의 전체 제목을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="f2055-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="f2055-113">검색은 대/소문자를 구분하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="f2055-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="f2055-114">검색 조건을 입력한 후 새로 고침 단추 새로 고침을 클릭하여 ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  결과를 필터링합니다.  </span><span class="sxs-lookup"><span data-stu-id="f2055-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="f2055-115">메시지와 파일을 확인 및 관리하는 데 사용하는 cmdlet은 다음을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="f2055-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="f2055-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="f2055-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="f2055-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="f2055-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="f2055-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="f2055-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="f2055-119">[Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)이 cmdlet은 SharePoint Online, 비즈니스용 OneDrive 또는 Teams에 대한 ATP의 맬웨어 파일이 아니라 메시지 전용입니다.</span><span class="sxs-lookup"><span data-stu-id="f2055-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="f2055-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="f2055-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)