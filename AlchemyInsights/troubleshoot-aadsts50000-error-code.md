---
title: AADSTS50000 오류 코드 문제 해결
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9801"
- "9005744"
ms.openlocfilehash: 63689ea5afea7c6921c93f2ead2350f87c2defa8
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898306"
---
# <a name="troubleshoot-aadsts50000-error-code"></a><span data-ttu-id="2b67e-102">AADSTS50000 오류 코드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="2b67e-102">Troubleshoot AADSTS50000 error code</span></span>

<span data-ttu-id="2b67e-103">AADSTS50000 오류를 해결하려면 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="2b67e-103">To resolve AADSTS50000 error, perform the following step:</span></span>

<span data-ttu-id="2b67e-104">**AADSTS50000**: TokenIssuanceError - 로그인 서비스에 문제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2b67e-104">**AADSTS50000**: TokenIssuanceError - There's an issue with the sign-in service.</span></span>

<span data-ttu-id="2b67e-105">액세스 토큰 요청이 유효하고 인증된 경우 인증 서버에서 액세스 토큰 및 선택적 새로 고침 토큰 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="2b67e-105">If the access token request is valid and authorized, the authorization server issues an access token and an optional refresh token.</span></span> <span data-ttu-id="2b67e-106">요청이 클라이언트 인증에 실패했거나 유효하지 않은 경우 인증 서버에서 오류 응답을 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="2b67e-106">If the request failed client authentication or is invalid, the authorization server returns an error response.</span></span>

<span data-ttu-id="2b67e-107">인증 서버에서 오류 코드와 다음 **오류** 매개 변수를 응답해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2b67e-107">The authorization server responds with an error code and includes the following **error** parameter with the response:</span></span>

`invalid_request: The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed.`

`invalid_client: Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method).  The authorization server MAY return an HTTP 401 (Unauthorized) status code to indicate which HTTP authentication schemes are supported.  If the client attempted to authenticate via the "Authorization" request header field, the authorization server MUST respond with an HTTP 401 (Unauthorized) status code and include the "WWW-Authenticate" response header field matching the authentication scheme used by the client.`

`invalid_grant: The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client.`

`unauthorized_client: The authenticated client is not authorized to use this authorization grant type.`

`unsupported_grant_type: The authorization grant type is not supported by the authorization server.`

`invalid_scope: The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner.`

<span data-ttu-id="2b67e-108">[지원 티켓 열기](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-troubleshooting-support-howto)를 사용하여 이 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2b67e-108">[Open a support ticket](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-troubleshooting-support-howto) to resolve this issue.</span></span>