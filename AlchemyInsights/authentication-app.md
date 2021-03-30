---
title: 인증 앱
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403837"
---
# <a name="authentication-app"></a><span data-ttu-id="ed986-102">인증 앱</span><span class="sxs-lookup"><span data-stu-id="ed986-102">Authentication app</span></span>

<span data-ttu-id="ed986-103">전역 관리자인 경우 로그인 진단 을 사용하여 발생된 문제를 빠르게 찾거나 사용자 로그인과 관련된 문제를 진단할 [수 있습니다.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="ed986-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="ed986-104">"진단 시작" 단추를 클릭하여[진단을](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)시작하세요.</span><span class="sxs-lookup"><span data-stu-id="ed986-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="ed986-105">사용자, 응용 프로그램, 로그인 시간, 요청 ID 또는 상관 관계 ID에 대한 세부 정보를 입력하여 분석할 이벤트를 찾아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ed986-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="ed986-106">필요한 경우 변경하기 위해 수행할 수 있는 작업과 작업에 대한 세부 정보를 보여주는 진단 결과를 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="ed986-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="ed986-107">**적용 가능한 시나리오를 검사합니다.**</span><span class="sxs-lookup"><span data-stu-id="ed986-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="ed986-108">사용자가 Microsoft Authenticator 앱에서 푸시 알림을 수신하지 않는 경우 사용자 차단 및 차단 해제에 설명된 MFA 차단된 사용자 아래에 해당 사용자가 표시되어 있지 [않은지 확인](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="ed986-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="ed986-109">사용자가 MFA에 대해 차단되지 않지만 푸시 알림을 받지 않는 경우 보류 중인 승인 요청을 끌어오는 Microsoft Authenticator 앱을 열 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ed986-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="ed986-110">다른 로그인 방법으로 로그인을 클릭하고 모바일 앱에서 확인 코드 사용을 선택할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ed986-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="ed986-111">Microsoft Authenticator 앱은 많은 사용자가 사용할 수 있는 유일한 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="ed986-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="ed986-112">[보안 기본값에 대한 자세한 내용은](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)인증자 앱 [FAQ에서](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) 자주 묻는 질문과 해결 방법을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ed986-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="ed986-113">**권장 비디오**</span><span class="sxs-lookup"><span data-stu-id="ed986-113">**Recommended Videos**</span></span>

<span data-ttu-id="ed986-114">[새 전화(2분)에 인증자](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)앱을 설정하는 방법</span><span class="sxs-lookup"><span data-stu-id="ed986-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
