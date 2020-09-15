---
title: Teams 클라이언트에 일정 아이콘이 표시되지 않음
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: f30cd5bda62756cf6b912ed150b4e59e7ca4d85d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684704"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="ae6db-102">Teams 클라이언트에 일정 아이콘이 표시되지 않음</span><span class="sxs-lookup"><span data-stu-id="ae6db-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="ae6db-103">Teams의 일정 탭은 Exchange 웹 서비스를 통한 Exchange 사서함에 대한 액세스를 필요로합니다.</span><span class="sxs-lookup"><span data-stu-id="ae6db-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="ae6db-104">Exchange 사서함은 온라인 이거나 온-프레미스 일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae6db-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="ae6db-105">일정 탭이 표시되지 않는 온라인 사용자의 경우 [Exchange Online 사서함에 대한 라이선스가 부여되고 사서함이 사용하도록 설정](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ae6db-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="ae6db-106">사용자에게 Exchange Online의 유효한 사서함이 있지만 여전히 일정 탭이 표시되지 않는 경우 네트워크 문제일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ae6db-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="ae6db-107">[Microsoft 원격 연결 분석기](https://testconnectivity.microsoft.com/)를 사용하여 영향받는 사용자에 대한 **Microsoft Exchange 웹 서비스 연결 테스트**를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="ae6db-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="ae6db-108">마지막으로 [Teams 앱 – 앱 설정 정책](https://admin.teams.microsoft.com/policies/app-setup)을 통해 사용자에게 적용되는 정책에서 일정 앱이 제거되지 않았는지 확인합니다 **(전역(조직 전체의 기본값)일 가능성 높음**.</span><span class="sxs-lookup"><span data-stu-id="ae6db-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="ae6db-109">사용자가 온-프레미스에 있는 경우 하이브리드 구성이 정상인지 확인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ae6db-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="ae6db-110">[하이브리드 구성 마법사](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)를 사용하여 문제를 해결하십시오.</span><span class="sxs-lookup"><span data-stu-id="ae6db-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="ae6db-111">[Teams는 Exchange 2016 CU3 이상을 필요](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)로 합니다.</span><span class="sxs-lookup"><span data-stu-id="ae6db-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
