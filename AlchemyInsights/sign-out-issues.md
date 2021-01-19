---
title: 로그 아웃 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886842"
---
# <a name="sign-out-issues"></a><span data-ttu-id="69097-102">로그 아웃 문제</span><span class="sxs-lookup"><span data-stu-id="69097-102">Sign-out issues</span></span>

<span data-ttu-id="69097-103">로그 아웃과 관련된 문제는 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="69097-103">To resolve issues related to signing out, perform the following steps:</span></span>

1. <span data-ttu-id="69097-104">사용자나 사용자가 응용 프로그램에서 로그아웃되거나 종료되는 경우 [조건별 액세스를 사용하여 인증 세션 관리 구성"](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime)또는 [Microsoft ID 플랫폼에서 토큰 수명 구성](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)의 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="69097-104">If you or a user are getting logged or kicked out of applications, follow the guidance in the articles [Configure authentication session management with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) or [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
2. <span data-ttu-id="69097-105">다른 대부분의 로그아웃 오류 또는 문제는 Azure AD(Azure Active Directory)를 특정 응용 프로그램과 통합하는 문제를 해결하여 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69097-105">Most other sign-out errors or problems can be solved by troubleshooting the integration of Azure Active Directory (Azure AD) with the specific application.</span></span> <span data-ttu-id="69097-106">다음을 포함한 [Azure Active Directory와 애플리케이션을 통합하기 위한 자습서 모음](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)으로 이동하여 특정 통합에 대한 지침을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69097-106">You can find guidance for a specific integration by going to this [collection of tutorials for integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), including:</span></span>
    - <span data-ttu-id="69097-107">SaaS 응용 프로그램 자습서</span><span class="sxs-lookup"><span data-stu-id="69097-107">SaaS application tutorials</span></span>
    - <span data-ttu-id="69097-108">Single Sign-On 자습서</span><span class="sxs-lookup"><span data-stu-id="69097-108">Single sign-on tutorials</span></span>
    - <span data-ttu-id="69097-109">사용자 프로비저닝 자습서</span><span class="sxs-lookup"><span data-stu-id="69097-109">User-provisioning tutorials</span></span>