---
title: 응용 프로그램 보호 정책
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 929400dcf0ca18ce8f52cb11e5c907064449480e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716899"
---
# <a name="application-protection-policy"></a><span data-ttu-id="7d082-102">응용 프로그램 보호 정책</span><span class="sxs-lookup"><span data-stu-id="7d082-102">Application protection policy</span></span>

<span data-ttu-id="7d082-103">APP(Application protection policy)에 처음이라면 [앱 보호 정책 개요](https://docs.microsoft.com/intune/apps/app-protection-policy)를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="7d082-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="7d082-104">APP 사용을 시작하려면 [앱 보호 정책 만들고 할당하는 방법](https://docs.microsoft.com/intune/app-protection-policies)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7d082-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="7d082-105">응용 프로그램 보호 정책 요구사항:</span><span class="sxs-lookup"><span data-stu-id="7d082-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="7d082-106">사용자가 Intune 또는 EMS 라이선스가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7d082-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="7d082-107">사용자가 응용 프로그램 보호 정책의 대상이 되는 그룹에 속해 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7d082-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="7d082-108">장치에서 보호되는 앱에 한 회사의 사용자만 로그인 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7d082-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="7d082-109">응용 프로그램에서 [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started)을 구현 했습니다.</span><span class="sxs-lookup"><span data-stu-id="7d082-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="7d082-110">SDK를 지원하는 앱 목록은 [Microsoft Intune 보호 앱](https://docs.microsoft.com/intune/apps-supported-intune-apps)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7d082-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="7d082-111">위의 요구 사항을 충족 하는 사용자가 Intune SDK를 사용 하는 앱에 로그인 하면 정책이 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="7d082-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="7d082-112">정책이 적용 되는지 확인 하는 가장 쉬운 방법은 사용자가 정책에서 PIN을 설정 하도록 요청 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="7d082-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="7d082-113">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7d082-113">For more information, see:</span></span>

[<span data-ttu-id="7d082-114">APP/MAM 문제 해결 FAQ</span><span class="sxs-lookup"><span data-stu-id="7d082-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="7d082-115">앱 보호 정책 설정의 유효성을 검사 하는 방법</span><span class="sxs-lookup"><span data-stu-id="7d082-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="7d082-116">앱 보호 정책에 전달 시간 이해</span><span class="sxs-lookup"><span data-stu-id="7d082-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="7d082-117">앱 보호 정책을 모니터링 하는 방법</span><span class="sxs-lookup"><span data-stu-id="7d082-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)