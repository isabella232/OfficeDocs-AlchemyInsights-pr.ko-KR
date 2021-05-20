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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539830"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="6f170-102">전자 메일이 없는 경우"</span><span class="sxs-lookup"><span data-stu-id="6f170-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="6f170-103">관리자는 이러한 메시지를 [보거나 해제하거나 삭제할 수 있습니다.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="6f170-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="6f170-104">보안 및 준수 & 열기 위해 로 이동 [https://protection.office.com](https://protection.office.com/) 합니다.</span><span class="sxs-lookup"><span data-stu-id="6f170-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="6f170-105">Quarantine 페이지를 직접 열기 위해 로 [https://protection.office.com/quarantine](https://protection.office.com/quarantine) 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="6f170-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="6f170-106">다음 값을 기준으로 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6f170-106">You can search by the following values:</span></span>  

- <span data-ttu-id="6f170-107">**메시지 ID**: 메시지의 GUID(Globally Unique Identifier)입니다.</span><span class="sxs-lookup"><span data-stu-id="6f170-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="6f170-108">목록에서 메시지를 선택하면 메시지  **ID**  값이 나타나는 세부 정보  **플라이아웃**  창에 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="6f170-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="6f170-109">관리자는 [메시지 추적](/microsoft-365/security/office-365-security/message-trace-scc)을 사용하여 메시지와 해당 메시지 ID 값을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6f170-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="6f170-110">**보낸 사람 전자 메일 주소**: 보낸 사람 한 명의 전자 메일 주소입니다.</span><span class="sxs-lookup"><span data-stu-id="6f170-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="6f170-111">**받는 사람 전자 메일 주소**: 받는 사람 한 명의 전자 메일 주소입니다.</span><span class="sxs-lookup"><span data-stu-id="6f170-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="6f170-112">**제목**: 메시지의 전체 제목을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="6f170-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="6f170-113">검색은 대/소문자를 구분하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6f170-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="6f170-114">검색 조건을 입력한 후 ![새로 고침 단추](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **새로 고침** 을 클릭하여 결과를 필터링합니다.</span><span class="sxs-lookup"><span data-stu-id="6f170-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="6f170-115">메시지와 파일을 확인 및 관리하는 데 사용하는 cmdlet은 다음을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="6f170-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="6f170-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="6f170-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="6f170-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="6f170-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="6f170-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="6f170-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="6f170-119">[Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)이 cmdlet은 Microsoft Defender에서 Office 365 Online, 비즈니스용 OneDrive SharePoint 또는 앱용 맬웨어 파일이 아니라 메시지에만 사용할 수 Teams.</span><span class="sxs-lookup"><span data-stu-id="6f170-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="6f170-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="6f170-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)