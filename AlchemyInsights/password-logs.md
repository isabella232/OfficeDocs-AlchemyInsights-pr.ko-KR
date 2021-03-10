---
title: 암호 로그
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
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523087"
---
# <a name="password-logs"></a><span data-ttu-id="c16a6-102">암호 로그</span><span class="sxs-lookup"><span data-stu-id="c16a6-102">Password logs</span></span>

<span data-ttu-id="c16a6-103">**암호 재설정 감사 로그에 액세스하는 데 문제가 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="c16a6-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="c16a6-104">암호 재설정 감사 로그 액세스와 관련한 문제를 해결하려면 다음 단계를 수행하세요.</span><span class="sxs-lookup"><span data-stu-id="c16a6-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="c16a6-105">감사 로그를 볼 권한이 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c16a6-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="c16a6-106">다음 역할에 한해 권한이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c16a6-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="c16a6-107">전역 관리자</span><span class="sxs-lookup"><span data-stu-id="c16a6-107">Global administrator</span></span>
 - <span data-ttu-id="c16a6-108">보안 관리자</span><span class="sxs-lookup"><span data-stu-id="c16a6-108">Security administrator</span></span>
 - <span data-ttu-id="c16a6-109">보안 읽기 권한자</span><span class="sxs-lookup"><span data-stu-id="c16a6-109">Security reader</span></span>

<span data-ttu-id="c16a6-110">**처음 배포한 때로부터 모든 암호 재설정 감사 이벤트를 보려는 경우**</span><span class="sxs-lookup"><span data-stu-id="c16a6-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="c16a6-111">최근 30일에 해당하는 보고서에 최대 120,000개의 암호 재설정/등록 이벤트가 저장됩니다.</span><span class="sxs-lookup"><span data-stu-id="c16a6-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="c16a6-112">이 최대 한도는 CSV를 다운로드할 때 UI에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="c16a6-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="c16a6-113">PowerShell을 통해 1백만 개 이벤트가 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="c16a6-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="c16a6-114">자세한 내용은 다음 링크를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c16a6-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="c16a6-115">Azure AD 보고서 및 이벤트 API의 셀프 서비스 암호 재설정 이벤트</span><span class="sxs-lookup"><span data-stu-id="c16a6-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c16a6-116">PowerShell을 사용하여 빠르게 암호 재설정 등록 이벤트를 다운로드하는 방법</span><span class="sxs-lookup"><span data-stu-id="c16a6-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="c16a6-117">**암호 재설정 보고 기능에 대한 자세한 정보를 알고 싶은 경우**</span><span class="sxs-lookup"><span data-stu-id="c16a6-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="c16a6-118">Microsoft Azure portal의 **사용자 및 그룹** 에서 Azure AD 암호 재설정 감사 로그를 사용하여 암호를 등록하거나 재설정하는 사람을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c16a6-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="c16a6-119">자세한 내용은 다음 링크를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c16a6-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="c16a6-120">암호 재설정 보고서 개요</span><span class="sxs-lookup"><span data-stu-id="c16a6-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c16a6-121">Azure Portal에서 암호 재설정 보고서를 보는 방법</span><span class="sxs-lookup"><span data-stu-id="c16a6-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c16a6-122">Azure AD 보고서 및 이벤트 API의 셀프 서비스 암호 재설정 이벤트</span><span class="sxs-lookup"><span data-stu-id="c16a6-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c16a6-123">PowerShell을 사용하여 빠르게 암호 재설정 등록 이벤트를 다운로드하는 방법</span><span class="sxs-lookup"><span data-stu-id="c16a6-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


