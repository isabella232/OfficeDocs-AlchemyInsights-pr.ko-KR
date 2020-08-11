---
title: Mac용 Teams 추가 기능
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2020
ms.locfileid: "46617104"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="c6a06-102">Mac용 Teams 추가 기능</span><span class="sxs-lookup"><span data-stu-id="c6a06-102">Teams add-in for Mac</span></span>

<span data-ttu-id="c6a06-103">누락된 Mac 운영 체제 사용자의 Teams 추가 기능 문제를 해결하려면 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="c6a06-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="c6a06-104">**1단계:** 하이브리드 Exchange On-Premises(2016 CU3  이상 필요)가 있는 경우 Test-HMA.ps1 도구를 사용하여 Hybrid Modern Authentication이 올바르게 구성되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c6a06-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="c6a06-105">자세한 내용은 [iOS 및 Android용 하이브리드 현대 인증 설정](https://aka.ms/AA980zq)을(를) 참조하시기 바랍니다.</span><span class="sxs-lookup"><span data-stu-id="c6a06-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="c6a06-106">**참고** domain\username이 아닌 UPN 주소 형식(예: [username@contoso.com](mailto:username@contoso.com))을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="c6a06-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="c6a06-107">Exchange Online 사서함을 사용하는 사용자에게도 이 작업을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="c6a06-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="c6a06-108">**2 단계:** 사용자가 Mac용 Outlook에서 **도구** > **계정**으로 이동하고 계정을 찾아서 선택하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6a06-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="c6a06-109">나열된 사용자 이름이 UPN 형식인지 확인합니다(예: [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="c6a06-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="c6a06-110">**3단계:** 사용자가 라이센스가 부여된 Microsoft Teams 사용자인지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c6a06-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="c6a06-111">사용자는 Mac용 Office 365 제품 버전 16.24 이상을 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c6a06-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>