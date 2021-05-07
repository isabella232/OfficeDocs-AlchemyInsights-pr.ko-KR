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
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233510"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="fa4d7-102">SharePoint에서 401 권한 없음 오류</span><span class="sxs-lookup"><span data-stu-id="fa4d7-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="fa4d7-p101">SharePoint에서 "(401) 권한 없음"이라는 오류가 표시될 경우, 이 문제는 TLS 1.0/1.1 사용 중단과 관련이 있을 수 있습니다. 자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="fa4d7-p101">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see:</span></span>

[<span data-ttu-id="fa4d7-105">Office 365 및 Office 365 GCC에서 TLS 1.2 준비</span><span class="sxs-lookup"><span data-stu-id="fa4d7-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[<span data-ttu-id="fa4d7-106">클라이언트에 TLS 1.2가 지원되지 않는 경우 인증 오류 발생</span><span class="sxs-lookup"><span data-stu-id="fa4d7-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="fa4d7-107">사용자가 Windows 7을 사용하는 경우 [Windows 7에서 TLS Cipher Suites](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)를 확인해야합니다.</span><span class="sxs-lookup"><span data-stu-id="fa4d7-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>