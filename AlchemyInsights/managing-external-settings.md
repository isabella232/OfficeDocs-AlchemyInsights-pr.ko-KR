---
title: 외부 설정 관리
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50282834"
---
# <a name="managing-external-settings"></a><span data-ttu-id="a4e9c-102">외부 설정 관리</span><span class="sxs-lookup"><span data-stu-id="a4e9c-102">Managing External Settings</span></span>

<span data-ttu-id="a4e9c-103">**알림**</span><span class="sxs-lookup"><span data-stu-id="a4e9c-103">**Announcement**</span></span>

- <span data-ttu-id="a4e9c-104">[2021년 1월 4일부터 Google의 WebView 로그인 지원을 중단합니다](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="a4e9c-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="a4e9c-105">호환성 테스트에 대한 Google의 지침을 따라 앱이 영향을 받는지 테스트합니다.</span><span class="sxs-lookup"><span data-stu-id="a4e9c-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="a4e9c-106">소비자 Google 계정으로 사용자를 로그인할 때 시스템 웹 보기 또는 시스템 브라우저를 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a4e9c-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="a4e9c-107">**초대 설정 관리**</span><span class="sxs-lookup"><span data-stu-id="a4e9c-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="a4e9c-108">적절한 사용자가 초대를 보낼 수 있도록 [외부 공동 작업 설정을 구성했는지](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="a4e9c-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="a4e9c-109">**게스트 사용자 액세스 권한 관리**</span><span class="sxs-lookup"><span data-stu-id="a4e9c-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="a4e9c-110">전역 관리자는 외부 공동 작업 설정 페이지에서 게스트 액세스 권한을 구성하여 Azure Portal을 통해 디렉터리의 게스트 액세스 권한을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a4e9c-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="a4e9c-111">[이 설정에 대해 자세히 알아보세요](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="a4e9c-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="a4e9c-112">게스트가 Teams 또는 SharePoint와 같은 앱에 액세스하도록 하려면 게스트 액세스를 허용하도록 해당 앱을 구성했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="a4e9c-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="a4e9c-113">[Teams 설정](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) 및 [Sharepoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)에 대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="a4e9c-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="a4e9c-114">**초대 구성:**</span><span class="sxs-lookup"><span data-stu-id="a4e9c-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="a4e9c-115">B2B 외부 공동 작업을 활성화하고 게스트를 초대할 수 있는 사용자 관리</span><span class="sxs-lookup"><span data-stu-id="a4e9c-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a4e9c-116">특정 조직의 사용자에 대한 초대 허용 또는 차단</span><span class="sxs-lookup"><span data-stu-id="a4e9c-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="a4e9c-117">**허용된 ID 공급자 구성:**</span><span class="sxs-lookup"><span data-stu-id="a4e9c-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="a4e9c-118">Google 페더레이션</span><span class="sxs-lookup"><span data-stu-id="a4e9c-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a4e9c-119">직접 페더레이션</span><span class="sxs-lookup"><span data-stu-id="a4e9c-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a4e9c-120">전자 메일 일회용 암호 인증</span><span class="sxs-lookup"><span data-stu-id="a4e9c-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
