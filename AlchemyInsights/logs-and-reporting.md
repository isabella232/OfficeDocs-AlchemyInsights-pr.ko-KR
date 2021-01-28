---
title: 로그 및 보고
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50031501"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="b6ef8-102">로그 및 보고</span><span class="sxs-lookup"><span data-stu-id="b6ef8-102">Logs and Reporting</span></span>

<span data-ttu-id="b6ef8-103">[Azure Active Directory 보고 FAQ는](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) Azure AD(Azure Active Directory) 보고에 대한 질문과 대답입니다.</span><span class="sxs-lookup"><span data-stu-id="b6ef8-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="b6ef8-104">자세한 내용은 [Azure Active Directory 보고를 참조하세요.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="b6ef8-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="b6ef8-105">**감사 문제 해결**</span><span class="sxs-lookup"><span data-stu-id="b6ef8-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="b6ef8-106">일부 감사 활동이 표시하는 데 문제가 있으며 누락된 활동이 이 목록에 있는 경우 [지원](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)티켓을 제출하세요.</span><span class="sxs-lookup"><span data-stu-id="b6ef8-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="b6ef8-107">테넌트에 감사 로그가 표시하는 데 문제가 있는 경우 지원 티켓을 제출하세요.</span><span class="sxs-lookup"><span data-stu-id="b6ef8-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="b6ef8-108">Azure Portal에 감사 활동이 즉시 표시되지 않는 [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) 경우 지연이 문서화된 대기 시간을 초과하는 경우 대기 시간 정보를 확인하고 지원 티켓을 제출하세요.</span><span class="sxs-lookup"><span data-stu-id="b6ef8-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="b6ef8-109">Azure AD 활동 로그 보존</span><span class="sxs-lookup"><span data-stu-id="b6ef8-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="b6ef8-110">선택한 날짜 범위에 대한 모든 감사가 표시되지 않는 경우 Azure Portal에서 최대 250K 행(가장 최근의 순서로 정렬)의 로그인을 다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b6ef8-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="b6ef8-111">자세한 내용은 감사 활동 [다운로드를 참조하세요.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="b6ef8-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="b6ef8-112">**로그인 문제 해결**</span><span class="sxs-lookup"><span data-stu-id="b6ef8-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="b6ef8-113">테넌트에 대한 Azure AD Premium(P1 또는 P2) 라이선스가 있는 경우 지난 30일간의 데이터만 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b6ef8-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="b6ef8-114">로그인은 Azure AD Premium 테넌트에만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b6ef8-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="b6ef8-115">무료 또는 기본 라이선스 테넌트에는 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b6ef8-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="b6ef8-116">테넌트에 Premium P1 라이선스가 있는 경우 로그인을 볼 수 없는 [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) 경우 지연 시간이 문서화된 대기 시간을 초과하는 경우 대기 시간 정보를 확인하고 지원 티켓을 제출하세요.</span><span class="sxs-lookup"><span data-stu-id="b6ef8-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="b6ef8-117">선택한 날짜 범위에 대한 모든 로그인이 표시되지 않는 경우 Azure Portal에서 최대 250K 행(가장 최근으로 정렬)의 로그인을 다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b6ef8-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="b6ef8-118">자세한 내용은 로그인 활동 [다운로드를 참조하세요.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="b6ef8-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="b6ef8-119">**보안 보고서 문제 해결(위험에 플래그가 지정되어 있는 사용자, 위험한 로그인)**</span><span class="sxs-lookup"><span data-stu-id="b6ef8-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="b6ef8-120">위험 보안 보고서에 플래그가 지정된 사용자</span><span class="sxs-lookup"><span data-stu-id="b6ef8-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="b6ef8-121">Azure Active Directory 포털의 위험한 로그인 보고서</span><span class="sxs-lookup"><span data-stu-id="b6ef8-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="b6ef8-122">Azure Active Directory 위험 이벤트</span><span class="sxs-lookup"><span data-stu-id="b6ef8-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
