---
title: 사용자 동의 문제 해결
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
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897762"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="d5e95-102">사용자 동의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="d5e95-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="d5e95-103">Azure Portal 또는 PowerShell을 통해 최종 사용자가 응용 프로그램에 동의하는 방법을 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5e95-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="d5e95-104">자세한 [내용은 사용자 동의](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) 설정을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d5e95-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="d5e95-105">관리자는 Microsoft Graph [API를](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) 사용하여 단일 사용자를 대신하여 위임된 사용 권한에 대한 동의를 부여할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d5e95-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="d5e95-106">자세한 내용은 사용자를 대신하여 [액세스](https://docs.microsoft.com/graph/auth-v2-user)권한을 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="d5e95-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="d5e95-107">[사용자 동의 오류:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)이 문서에서는 응용 프로그램에 동의하는 프로세스 중에 발생할 수 있는 오류에 대해 논의합니다.</span><span class="sxs-lookup"><span data-stu-id="d5e95-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="d5e95-108">오류 메시지가 포함되지 않은 예기치 않은 동의 프롬프트 문제를 해결하는 경우 Azure AD에 대한 [인증 시나리오를 참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)</span><span class="sxs-lookup"><span data-stu-id="d5e95-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>