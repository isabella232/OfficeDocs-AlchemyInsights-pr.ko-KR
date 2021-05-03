---
title: Windows 7 컴퓨터의 SharePoint 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067000"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Windows 7 컴퓨터의 SharePoint 문제

SharePoint 또는 OneDrive에서 작업하는 동안 Windows 7 컴퓨터에서 오류가 발생하는 경우 TLS 1.0/1.1의 사용 중단과 관련이 있을 수 있습니다. 자세한 내용은 다음을 참조하세요.

- [Office 365 및 Office 365 GCC에서 TLS 1.2 준비](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 클라이언트에는 TLS1.2가 사용하도록 설정되어 있어야 합니다. 자세한 내용은 [클라이언트에 TLS 1.2가 지원되지 않는 경우 인증 오류 발생](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)을 참조하세요.

- KB3140245를 설치하고 레지스트리 값을 생성합니다. 자세한 내용은  [Windows의 WinHTTP에서 기본 보안 프로토콜로 TLS 1.1 및 TLS 1.2를 사용하도록 업데이트](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)를 참조하세요.

- Windows 7 SP1/Windows 8 클라이언트에는 최신 TLS 암호 제품군이 설치되어 있어야 합니다. 자세한 내용은 [Microsoft 보안 공지 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058)을 참조하세요. 


