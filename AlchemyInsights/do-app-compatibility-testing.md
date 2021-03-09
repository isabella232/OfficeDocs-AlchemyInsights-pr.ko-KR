---
title: 앱 호환성 테스트 수행
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530136"
---
# <a name="do-app-compatibility-testing"></a><span data-ttu-id="dd0d5-102">앱 호환성 테스트 수행</span><span class="sxs-lookup"><span data-stu-id="dd0d5-102">Do app compatibility testing</span></span>

<span data-ttu-id="dd0d5-103">Microsoft Edge의 애플리케이션 호환성은 매우 높습니다.</span><span class="sxs-lookup"><span data-stu-id="dd0d5-103">Application compatibility for Microsoft Edge is extremely high.</span></span> <span data-ttu-id="dd0d5-104">실제로 Microsoft는 다음과 같은 호환성 약속을 제공할 정도로 매우 높습니다.</span><span class="sxs-lookup"><span data-stu-id="dd0d5-104">In fact, it's so high that Microsoft provides the following compatibility promises:</span></span>
- <span data-ttu-id="dd0d5-105">Microsoft Edge 45 이상 버전에서 작동하면 Microsoft Edge 77 이상 버전에서 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="dd0d5-105">If it works on Microsoft Edge 45 and earlier versions, it will work on Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="dd0d5-106">Internet Explorer에서 작동하면 Internet Explorer 모드의 Microsoft Edge에서 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="dd0d5-106">If it works on Internet Explorer, it will work on Microsoft Edge in Internet Explorer mode.</span></span>
- <span data-ttu-id="dd0d5-107">Google Chrome 에서 작동하면 Microsoft Edge 에서도 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="dd0d5-107">If it works on Google Chrome, it will work on Microsoft Edge.</span></span>

<span data-ttu-id="dd0d5-108">이러한 약속을 충족하지 않는 애플리케이션이 있는 경우 [ Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure)로 이러한 약속을 수정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd0d5-108">If you have an application where we don't meet this promise, then we stand behind the promise to fix it with [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span></span>

<span data-ttu-id="dd0d5-109">이러한 약속에도 불구하고 많은 조직은 규정 준수 또는 위험 관리상의 이유로 일부 애플리케이션의 유효성을 확인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="dd0d5-109">Despite this promise, we know that many organizations must validate some applications for compliance or risk-management reasons.</span></span> <span data-ttu-id="dd0d5-110">이러한 확인 작업은 매우 간단할 것으로 예상되지만, 앱 테스트은 체계적이고 엄격한 태도로 진행하는 것이 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="dd0d5-110">Even though we expect this to be very straightforward, it's important to be organized and rigorous in app testing.</span></span>

<span data-ttu-id="dd0d5-111">앱 호환성 테스트를 수행하는 두 가지 방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="dd0d5-111">There are two ways to do app compatibility testing:</span></span>

- <span data-ttu-id="dd0d5-112">**랩 테스트**: 애플리케이션은 특정 구성으로 엄격한 제어를 받는 환경에서 테스트됩니다.</span><span class="sxs-lookup"><span data-stu-id="dd0d5-112">**Lab testing**: Applications are tested in a tightly controlled environment with specific configurations.</span></span>
- <span data-ttu-id="dd0d5-113">**파일럿 테스트**: 애플리케이션이 자신의 장치를 사용하여 일일 작업 환경에서 제한된 수의 사용자에 의해 테스트됩니다.</span><span class="sxs-lookup"><span data-stu-id="dd0d5-113">**Pilot testing**: Applications are tested by a limited number of users in their daily work environment using their own devices.</span></span>

<span data-ttu-id="dd0d5-114">각 앱에 가장 적합한 방법을 선택하고 전체 조직에 대해 시작하기 전에 테스트를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="dd0d5-114">Choose the method that is most appropriate for each app and do the testing prior to a launch to the entire organization.</span></span>

<span data-ttu-id="dd0d5-115">앱이 호환되는지 확인했다면 Microsoft Edge를 파일럿 그룹에 배포할 준비가 된 것입니다.</span><span class="sxs-lookup"><span data-stu-id="dd0d5-115">Once you've ensured that your apps are compatible, you're ready to deploy Microsoft Edge to a pilot group.</span></span>
