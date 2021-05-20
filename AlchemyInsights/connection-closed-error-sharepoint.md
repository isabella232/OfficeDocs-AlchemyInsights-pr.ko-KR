---
title: SharePoint의 기본 연결이 닫힘 오류
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 0515ead28cdfdbdb9529c269b5170b294ab2b120
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543043"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="213e5-102">SharePoint의 "기본 연결이 닫혀 있습니다" 오류</span><span class="sxs-lookup"><span data-stu-id="213e5-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="213e5-p101">SharePoint에서 "기존 연결이 닫혔습니다"라는 오류가 표시될 경우, 이 문제는 TLS 1.0/1.1 사용 중단과 관련이 있을 수 있습니다. 자세한 내용은 다음 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="213e5-p101">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see these articles:</span></span>

- [<span data-ttu-id="213e5-105">Office 365 및 Office 365 GCC에서 TLS 1.2 준비</span><span class="sxs-lookup"><span data-stu-id="213e5-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="213e5-106">클라이언트에 TLS 1.2가 지원되지 않는 경우 인증 오류 발생</span><span class="sxs-lookup"><span data-stu-id="213e5-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="213e5-107">Windows의 WinHTTP에서 기본 보안 프로토콜로 TLS 1.1 및 TLS 1.2를 사용하도록 업데이트</span><span class="sxs-lookup"><span data-stu-id="213e5-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="213e5-108">사용자가 Windows 7을 사용하는 경우 [Windows 7에서 TLS Cipher Suites](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)를 확인해야합니다.</span><span class="sxs-lookup"><span data-stu-id="213e5-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>