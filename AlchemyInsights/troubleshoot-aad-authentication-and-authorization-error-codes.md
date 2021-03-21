---
title: AADSTS(Azure AD 인증 및 권한 부여) 오류 코드 문제 해결
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
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898311"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="be468-102">AADSTS(Azure AD 인증 및 권한 부여) 오류 코드 문제 해결</span><span class="sxs-lookup"><span data-stu-id="be468-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="be468-103">AAD 인증 및 권한 부여(AADSTS) 오류 코드를 해결하기 위해 다음 권장 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="be468-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="be468-104">**응용 프로그램에서 오류 코드 처리**</span><span class="sxs-lookup"><span data-stu-id="be468-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="be468-105">**OAuth2.0 사양**, https://tools.ietf.org/html/rfc6749#section-5.2,는 오류 응답의 오류 부분을 사용하여 인증 중에 오류를 처리하는 방법에 대한 지침을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="be468-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="be468-106">**오류**: 발생하는 오류 유형을 분류하는 데 사용할 수 있으며 오류에 대응하는 데 사용할 수 있는 오류 코드 문자열입니다.</span><span class="sxs-lookup"><span data-stu-id="be468-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="be468-107">**오류** 필드에 여러 값을 사용할 수 있습니다. 특정 오류에 대한 자세한 정보와 그에 대응하는 방법에 대한 자세한 내용은 프로토콜 설명서 링크 및 OAuth 2.0 사양을 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="be468-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="be468-108">다음은 오류 응답 예제입니다.</span><span class="sxs-lookup"><span data-stu-id="be468-108">Here is a sample error response:</span></span>
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. <span data-ttu-id="be468-109">**현재 오류 코드 정보 보기**</span><span class="sxs-lookup"><span data-stu-id="be468-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="be468-110">오류 코드와 메시지는 변경될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="be468-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="be468-111">최신 정보는 https://login.microsoftonline.com/error 페이지에서 AADSTS 오류 설명, 수정 및 제안된 해결 방법을 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="be468-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="be468-112">[AADSTS 오류 코드](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes)는 게시물 [Azure AD 인증 및 권한 부여 오류 코드](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)에 목록이 기재되어 있으며, 검색하여 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="be468-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="be468-113">**도움말 보기**</span><span class="sxs-lookup"><span data-stu-id="be468-113">**Get Help**</span></span>

- <span data-ttu-id="be468-114">[개발자를 위한 지원 및 도움 옵션](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - 질문에 대한 답변이나 문서에 설명되어 있지 않은 문제를 해결하기 위해 도움이 필요한 경우 전문가에게 도움을 청해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="be468-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="be468-115">이 문서에서는 Microsoft ID 플랫폼과 통합되는 앱을 개발할 때 질문에 대한 답변을 얻기 위한 몇 가지 제안을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="be468-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








