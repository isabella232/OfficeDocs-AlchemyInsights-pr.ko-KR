---
title: 감사 로그에서 메시지 삭제 이벤트 확인
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508994"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="157e0-102">삭제 된 전자 메일 메시지에 대 한 감사 로그</span><span class="sxs-lookup"><span data-stu-id="157e0-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="157e0-103">2019 년 1 월부터 Microsoft는 기본적으로 사서함 감사 로깅을 설정 하 고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="157e0-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="157e0-104">그렇지 않고 특정 사용자에 대 한 메시지 삭제 이벤트를 검토 하려면 감사에 대 한 삭제 작업을 수동으로 사용 하도록 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="157e0-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="157e0-105">조직 또는 특정 사용자에 대해 사서함 감사 로깅이 이미 사용 하도록 설정 된 경우에는 아래 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="157e0-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="157e0-106">[Microsoft 365 보안 & 준수 센터](https://protection.office.com/) 에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="157e0-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="157e0-107">**검색 및 조사** 를 클릭 하 고 **감사 로그 검색**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="157e0-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="157e0-108">**시작 날짜** 및 **끝 날짜** 필드에서 날짜 범위를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="157e0-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="157e0-109">조사 하려는 사용자에 대 한 사용자 이름 (항목을 삭제 한 사용자)을 지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="157e0-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="157e0-110">**작업** 필드에서 **지운 편지함 폴더에서 삭제 된 메시지** 를 선택 하 고 **메시지를 지운 편지함 폴더로 이동**합니다.</span><span class="sxs-lookup"><span data-stu-id="157e0-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="157e0-111">**검색**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="157e0-111">Click **Search**.</span></span>

<span data-ttu-id="157e0-112">결과에서 감사 레코드를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="157e0-112">In the results, select an audit record.</span></span> <span data-ttu-id="157e0-113">세부 정보 플라이 아웃에서 **추가 정보**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="157e0-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="157e0-114">삭제 된 항목에 대 한 추가 정보 (예: 제목 줄 및 삭제 시 항목의 위치)가 **AffectedItems** 필드에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="157e0-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="157e0-115">**Clientinfostring** 속성은 outlook, 웹에서 outlook (이전의 Outlook web App) 또는 다른 모든 장치에서 삭제를 수행 했는지 여부를 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="157e0-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="157e0-116">자세한 내용은 [사서함에 대 한 전자 메일 전달을 설정한 사용자 결정](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="157e0-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="157e0-117">**참고**: 감사 로그 기능을 사용 하 여 삭제 된 항목을 검색할 수는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="157e0-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="157e0-118">웹용 Outlook에서 삭제 된 메시지를 검색 하려면 [Outlook Web App에서 삭제 된 항목 복구](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="157e0-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
