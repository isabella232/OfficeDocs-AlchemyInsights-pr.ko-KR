---
title: 감사 로그에서 IP 주소 및 클라이언트 식별
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668316"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="a1655-102">감사 로그에서 IP 주소 및 클라이언트 식별</span><span class="sxs-lookup"><span data-stu-id="a1655-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="a1655-103">Microsoft 365 사용자 또는 관리자가 수행한 활동에 해당 하는 IP 주소가 감사 로그에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a1655-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="a1655-104">클라이언트 정보도 기록 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a1655-104">The client information is also logged.</span></span> <span data-ttu-id="a1655-105">이러한 정보를 식별 하는 단계는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="a1655-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="a1655-106">[Microsoft 365 보안 & 준수 센터](https://protection.office.com/)에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a1655-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="a1655-107">**검색**  >  **감사 로그 검색** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="a1655-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="a1655-108">특정 활동에 관심이 있는 경우 **작업** 목록에서 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="a1655-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="a1655-109">그렇지 않으면 선택한 사용자에 대 한 모든 작업이 반환 됩니다 (기본 설정).</span><span class="sxs-lookup"><span data-stu-id="a1655-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="a1655-110">**참고**: 특정 활동은 **활동** 메뉴에서 사용 하지 못할 수 있습니다. 그러나 **모든 작업에 대 한 결과 표시** (기본 설정)가 선택 되어 있으면 이러한 감사 항목이 반환 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a1655-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="a1655-111">**사용자** 필드에서 사용자 이름을 지정 하 고 활동에 적합 한 날짜 범위를 선택한 다음 **검색**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a1655-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="a1655-112">결과 창에서 해당 활동의 IP 주소를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a1655-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="a1655-113">감사 레코드를 선택 하 여 **세부** 정보 플라이 아웃 (예: 클라이언트, 작업을 수행한 사용자)에서 자세한 내용을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a1655-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="a1655-114">자세한 내용은 [손상 된 계정에 액세스 하는 데 사용 되는 컴퓨터의 IP 주소 찾기를](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="a1655-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
