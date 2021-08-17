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
ms.openlocfilehash: f0f82eaaa00d71992af445bb89346fb85bad3ade5d120b25ad3a6ea4f9674893
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883325"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>SharePoint의 "기본 연결이 닫혀 있습니다" 오류

SharePoint에서 "기존 연결이 닫혔습니다"라는 오류가 표시될 경우, 이 문제는 TLS 1.0/1.1 사용 중단과 관련이 있을 수 있습니다. 자세한 내용은 다음 문서를 참조하세요.

- [Office 365 및 Office 365 GCC에서 TLS 1.2 준비](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [클라이언트에 TLS 1.2가 지원되지 않는 경우 인증 오류 발생](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Windows의 WinHTTP에서 기본 보안 프로토콜로 TLS 1.1 및 TLS 1.2를 사용하도록 업데이트](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

사용자가 Windows 7을 사용하는 경우 [Windows 7에서 TLS Cipher Suites](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)를 확인해야합니다.