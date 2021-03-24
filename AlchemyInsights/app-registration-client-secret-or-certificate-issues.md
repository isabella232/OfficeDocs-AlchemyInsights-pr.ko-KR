---
title: 앱 등록 클라이언트 비밀 또는 인증서 문제
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123201"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="02cda-102">앱 등록 클라이언트 비밀 또는 인증서 문제</span><span class="sxs-lookup"><span data-stu-id="02cda-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="02cda-103">응용 프로그램 클라이언트 비밀 만료 여부</span><span class="sxs-lookup"><span data-stu-id="02cda-103">Application client secret expiring?</span></span>

<span data-ttu-id="02cda-104">앱 등록 포털의 표준 등록 프로세스를 통해 또는 응용 프로그램 동의를 사용하여 테넌트에서 서비스 계정을 만든 경우 등록된 응용 프로그램을 만든 방식에 관계없이 현재 클라이언트 보안이 만료 전에 새 클라이언트 비밀을 만들어 관련 응용 프로그램 코드에서 업데이트해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02cda-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="02cda-105">최대 유효 기간은 2년입니다.</span><span class="sxs-lookup"><span data-stu-id="02cda-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="02cda-106">미리 알림으로 비밀 값은 포털에서 앱 등록 페이지를 종료한 후 더 이상 표시되지 않는 것으로 기록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="02cda-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="02cda-107">자세한 내용은 [빠른 시작: Microsoft ID](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) 플랫폼에서 앱 등록 및 Microsoft ID 플랫폼에 대한 모범 [사례를 참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="02cda-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="02cda-108">자세한 내용은 [Create an Azure AD app & service principal in the portal - Microsoft identity platform를 참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="02cda-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
