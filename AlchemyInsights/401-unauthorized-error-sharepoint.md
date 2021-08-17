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
ms.openlocfilehash: 8935f461aaf24cb100516311203ef642f5dbed931e472df944c1cd7e72a8cf4e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890272"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>SharePoint에서 401 권한 없음 오류

SharePoint에서 "(401) 권한 없음"이라는 오류가 표시될 경우, 이 문제는 TLS 1.0/1.1 사용 중단과 관련이 있을 수 있습니다. 자세한 내용은 다음을 참조하세요.

- [Office 365 및 Office 365 GCC에서 TLS 1.2 준비](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [클라이언트에 TLS 1.2가 지원되지 않는 경우 인증 오류 발생](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Windows의 WinHTTP에서 기본 보안 프로토콜로 TLS 1.1 및 TLS 1.2를 사용하도록 업데이트](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

사용자가 Windows 7을 사용하는 경우 [Windows 7에서 TLS Cipher Suites](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)를 확인해야합니다.