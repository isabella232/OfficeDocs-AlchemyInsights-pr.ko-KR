---
title: 액세스 토큰 가져오기 관련 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7776"
- "9004351"
ms.openlocfilehash: e2d15603835d3fb43df1b6b5dadec64af00290ff
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49912033"
---
# <a name="issues-with-getting-access-tokens"></a><span data-ttu-id="d2aa3-102">액세스 토큰 가져오기 관련 문제</span><span class="sxs-lookup"><span data-stu-id="d2aa3-102">Issues with getting access tokens</span></span>

<span data-ttu-id="d2aa3-103">이 토픽에서는 리소스에 액세스하기 위한 액세스 토큰을 획득하지 못하는 경우를 다룹니다.</span><span class="sxs-lookup"><span data-stu-id="d2aa3-103">This topic deals with failures to acquire access tokens to access a resource.</span></span>

<span data-ttu-id="d2aa3-104">**시작하는 데 문제가 있는 경우**</span><span class="sxs-lookup"><span data-stu-id="d2aa3-104">**I'm having trouble getting started**</span></span>

<span data-ttu-id="d2aa3-105">시작하려고 할 때 발생하는 문제를 해결하려면 다음 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d2aa3-105">To troubleshoot issues you encounter when trying to get started, see the following articles:</span></span>

- [<span data-ttu-id="d2aa3-106">시작할 코드 샘플을 찾을 수 없는 경우</span><span class="sxs-lookup"><span data-stu-id="d2aa3-106">I can't find a code sample to get started</span></span>](https://docs.microsoft.com/azure/active-directory/develop/sample-v2-code) 
- [<span data-ttu-id="d2aa3-107">.NET에서 토큰을 받는 데 도움이 필요한 경우</span><span class="sxs-lookup"><span data-stu-id="d2aa3-107">I need help getting a token in .NET</span></span>](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios)

<span data-ttu-id="d2aa3-108">**토큰을 요청하고 사용하는 방법을 모르는 경우**</span><span class="sxs-lookup"><span data-stu-id="d2aa3-108">**I don't know how to request and use tokens**</span></span>

<span data-ttu-id="d2aa3-109">토큰 요청 및 사용 방법에 대한 지침은 다음 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d2aa3-109">For guidance on how to request and use tokens, see the following articles:</span></span>

- [<span data-ttu-id="d2aa3-110">인증 코드를 요청하는 방법을 모르는 경우</span><span class="sxs-lookup"><span data-stu-id="d2aa3-110">I don’t know how to request an authorization code</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#request-an-authorization-code) 
- [<span data-ttu-id="d2aa3-111">액세스 토큰을 요청하는 방법을 모르는 경우</span><span class="sxs-lookup"><span data-stu-id="d2aa3-111">I don’t know how to request an access token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-authorization-code-to-request-an-access-token) 
- [<span data-ttu-id="d2aa3-112">액세스 토큰을 사용하여 리소스에 액세스하는 방법을 모르는 경우</span><span class="sxs-lookup"><span data-stu-id="d2aa3-112">I don’t know how to use an access token to access a resource</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-access-token-to-access-the-resource) 
- [<span data-ttu-id="d2aa3-113">액세스 토큰을 새로 고치는 방법을 모르는 경우</span><span class="sxs-lookup"><span data-stu-id="d2aa3-113">I don’t know how to refresh an access token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refreshing-the-access-tokens)

<span data-ttu-id="d2aa3-114">**토큰을 요청하는 동안 오류가 발생한 경우**</span><span class="sxs-lookup"><span data-stu-id="d2aa3-114">**I got an error while requesting a token**</span></span>

<span data-ttu-id="d2aa3-115">토큰을 요청하는 동안 발생한 오류를 해결하려면 다음 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d2aa3-115">To troubleshoot errors you have encountered while requesting for a token, see the following articles:</span></span>

- [<span data-ttu-id="d2aa3-116">토큰을 요청할 때 서비스 오류가 발생한 경우</span><span class="sxs-lookup"><span data-stu-id="d2aa3-116">I received a service error when requesting a token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- [<span data-ttu-id="d2aa3-117">이전에 작업한 앱에 새 오류가 발생하는 경우</span><span class="sxs-lookup"><span data-stu-id="d2aa3-117">I'm getting a new error to a previously working app</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-breaking-changes)

<span data-ttu-id="d2aa3-118">**AADSTS 오류 코드에 대한 자세한 정보를 받을 수 있는 방법**</span><span class="sxs-lookup"><span data-stu-id="d2aa3-118">**How do I get more information about AADSTS error codes?**</span></span>

<span data-ttu-id="d2aa3-119">자세한 내용은 [오류 코드 인증](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)을 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="d2aa3-119">For more information, see [Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes).</span></span>





