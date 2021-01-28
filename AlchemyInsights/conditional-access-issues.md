---
title: 조건부 액세스 문제
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013979"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="23d18-102">조건부 액세스 문제</span><span class="sxs-lookup"><span data-stu-id="23d18-102">Conditional access issues</span></span>

<span data-ttu-id="23d18-103">**로그인 진단 문제 해결**</span><span class="sxs-lookup"><span data-stu-id="23d18-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="23d18-104">로그인 진단을 사용하여 발생된 문제를 빠르게 찾거나 사용자 로그인과 관련된 문제를 [진단할 수 있습니다.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="23d18-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="23d18-105">로그인 진단을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="23d18-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="23d18-106">사용자, 응용 프로그램, 로그인 시간, 요청 ID 또는 상관 관계 ID에 대한 세부 정보를 입력하여 분석할 이벤트를 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="23d18-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="23d18-107">수행된 작업 및 변경을 위해 수행할 수 있는 작업(변경이 필요한 경우)에 대한 세부 정보를 표시하는 진단 결과를 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="23d18-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="23d18-108">**로그인 문제 해결 단계**</span><span class="sxs-lookup"><span data-stu-id="23d18-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="23d18-109">Azure AD 로그인 페이지로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="23d18-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="23d18-110">사용자, 시간 범위, 응용 프로그램, 상태, 클라이언트 앱 등으로 로그인을 필터링합니다.</span><span class="sxs-lookup"><span data-stu-id="23d18-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="23d18-111">로그인 이벤트를 선택하고 조건부 액세스 탭을 보고 평가된 정책을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="23d18-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="23d18-112">정책의 행을 클릭하여 정책 세부 정보를 보고 정책이 적용된 이유를 이해합니다.</span><span class="sxs-lookup"><span data-stu-id="23d18-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="23d18-113">**조건부 액세스 정책 문제 해결 도구**</span><span class="sxs-lookup"><span data-stu-id="23d18-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="23d18-114">보고서 전용 모드를 사용하면 사용자에게 영향을 주지 않고 정책을 평가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="23d18-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="23d18-115">가상 도구를 사용하면 로그인 이벤트를 시뮬레이트하고 적용되는 정책을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="23d18-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="23d18-116">인사이트 및 보고 통합 문서는 각 정책에 대한 실시간 영향을 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="23d18-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="23d18-117">**기준 보호 정책**</span><span class="sxs-lookup"><span data-stu-id="23d18-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="23d18-118">기준 보호 정책은 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="23d18-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="23d18-119">더 이상 적용되지는 않습니다. Azure Portal에서 곧 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="23d18-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="23d18-120">보안 기본값을 [사용하도록 설정하는 것이 좋습니다.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="23d18-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="23d18-121">조건부 액세스에 대한 자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="23d18-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="23d18-122">[Azure Active Directory의](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 조건부 액세스 모범 사례  
 [조건부 액세스 조건](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [조건부 액세스의 컨트롤](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [조건부 액세스의 위치](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="23d18-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
