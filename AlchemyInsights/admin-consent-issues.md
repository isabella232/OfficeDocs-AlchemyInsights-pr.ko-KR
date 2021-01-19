---
title: 관리자 동의 문제
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49888321"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="8adbb-102">관리자 동의 문제</span><span class="sxs-lookup"><span data-stu-id="8adbb-102">Admin consent issues</span></span>

1. <span data-ttu-id="8adbb-103">사용자가 [동의 화면에서](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) 직접 관리자 승인을 요청할 수 있도록 관리자 동의 워크플로를 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="8adbb-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="8adbb-104">사용자 또는 응용 프로그램의 사용자에게 동의 프로세스 중에 예기치 않은 오류가 발생하는 경우 이 문서를 참조하여 문제 해결 단계를 [참조하세요. 응용](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)프로그램에 동의할 때 예기치 않은 오류입니다.</span><span class="sxs-lookup"><span data-stu-id="8adbb-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="8adbb-105">[Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)ID 플랫폼의 관리자 동의, 동의 [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) 프롬프트가 작동하는 방식 및 테넌트 전체 관리자 동의 요청을 평가하는 방법에 [대해 자세히 알아보습니다.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="8adbb-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="8adbb-106">Microsoft ID 플랫폼과 통합되는 응용 프로그램은 사용자와 관리자가 데이터 액세스 방법을 제어할 수 있는 권한 부여 모델을 따르게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8adbb-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="8adbb-107">권한 부여 모델의 구현은 Microsoft ID 플랫폼 끝점에서 업데이트되고 앱이 Microsoft ID 플랫폼과 상호 작용하는 방법을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="8adbb-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="8adbb-108">범위, 사용 권한 및 동의를 포함하여 이 권한 부여 모델의 개요는 [Microsoft ID](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) 플랫폼 끝점의 사용 권한 및 동의를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8adbb-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>