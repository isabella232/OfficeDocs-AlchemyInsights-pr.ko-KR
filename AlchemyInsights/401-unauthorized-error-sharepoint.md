---
title: SharePoint에서 401 권한 없음 오류
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539938"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="1907d-102">SharePoint에서 401 권한 없음 오류</span><span class="sxs-lookup"><span data-stu-id="1907d-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="1907d-p101">SharePoint에서 "(401) 권한 없음"이라는 오류가 표시될 경우, 이 문제는 TLS 1.0/1.1 사용 중단과 관련이 있을 수 있습니다. 자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1907d-p101">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see:</span></span>

- [<span data-ttu-id="1907d-105">Office 365 및 Office 365 GCC에서 TLS 1.2 준비</span><span class="sxs-lookup"><span data-stu-id="1907d-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="1907d-106">클라이언트에 TLS 1.2가 지원되지 않는 경우 인증 오류 발생</span><span class="sxs-lookup"><span data-stu-id="1907d-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="1907d-107">Windows의 WinHTTP에서 기본 보안 프로토콜로 TLS 1.1 및 TLS 1.2를 사용하도록 업데이트</span><span class="sxs-lookup"><span data-stu-id="1907d-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="1907d-108">사용자가 Windows 7을 사용하는 경우 [Windows 7에서 TLS Cipher Suites](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)를 확인해야합니다.</span><span class="sxs-lookup"><span data-stu-id="1907d-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>