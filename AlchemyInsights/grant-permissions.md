---
title: 사용 권한 부여
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
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897755"
---
# <a name="grant-permissions"></a><span data-ttu-id="89e97-102">사용 권한 부여</span><span class="sxs-lookup"><span data-stu-id="89e97-102">Grant permissions</span></span>

1. <span data-ttu-id="89e97-103">테넌트 전체 관리자 동의 [](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) **부여:** Azure Portal, Azure AD PowerShell 사용 또는 동의 프롬프트 자체에서 테넌트 전체 관리자 동의를 부여하기 위한 단계별 지침은 테넌트 전체 관리자 동의를 응용 프로그램에 부여하세요.</span><span class="sxs-lookup"><span data-stu-id="89e97-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="89e97-104">**특정** 사용자 대신 동의 부여: 관리자는 전체 조직에 대한 동의를 부여하는 대신 [Microsoft Graph API를](https://docs.microsoft.com/graph/use-the-api) 사용하여 단일 사용자를 대신하여 위임된 사용 권한에 대한 동의를 부여할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="89e97-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="89e97-105">자세한 내용은 사용자를 대신하여 [액세스](https://docs.microsoft.com/graph/auth-v2-user)권한을 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="89e97-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>