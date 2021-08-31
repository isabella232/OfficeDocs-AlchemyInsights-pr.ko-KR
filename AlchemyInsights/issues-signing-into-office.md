---
title: 앱에 로그인하는 Microsoft 365 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744652"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>로그인하는 Microsoft 365 앱

참고: 이전 버전의 Windows(예: Windows 7 SP1, Windows Server 2008 R2)를 사용하는 경우 간단한 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) 수정을 사용하여 TLS 1.2를 기본값으로 사용하도록 설정하십시오. 자세한 내용은 [Windows의 WinHTTP에서 기본 보안 프로토콜로 TLS 1.1 및 TLS 1.2를 사용하도록 업데이트](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)를 참조하세요.

Microsoft 365 앱 관련 로그인 문제를 해결하려면 문제가 발생하는 컴퓨터에서 다음 옵션을 시도해 보세요.  

- 자세한 Windows 일반적인 권장 사항 해결에 대한 자세한 내용은 다음을 [참조합니다.](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- For Mac, see [Can't sign in to an Mac용 Office 2016 app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**팁** Windows 컴퓨터에서 몇 가지 일반적인 Office 로그인 문제를 자동으로 진단하고 해결해드립니다. 자동화된 도구를 사용하려면 **[Office 365 지원 및 복구 도우미](https://aka.ms/SaRA-OfficeSignInScenario)** 를 다운로드하고 실행하십시오.

**참고:** 로그인 또는 정품 인증 문제를 해결하기 위해 ADAL(최신 인증) 또는 WAM(웹 계정 관리)을 사용 안 하도록 설정하는 것은 **권장되지 않습니다.** Microsoft 365 2013을 사용하여 Office 연결하는 동안 오류가 발생하는 경우 클라이언트에 [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) 대해 최신 인증을 사용하도록 Office 합니다.

특정 문제 해결 작업에 대한 자세한 내용은 다음을 참조합니다.

[Windows 10에서 Office 2016 빌드 16.0.7967로 업데이트한 후 로그인 시 연결 문제](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[조직 계정(예: Office 365, Azure 또는 Intune)에 로그인할 수 없습니다.](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Office 365, Azure 또는 Intune에 로그인할 수 없는 비 브라우저 앱 문제를 해결하는 방법](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[2016에서 자격 증명을 입력하라는 메시지가 반복적으로 Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)