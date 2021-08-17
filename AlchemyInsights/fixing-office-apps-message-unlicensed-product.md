---
title: Office를 정품 인증할 수 없습니다
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
- "2000023"
- "3509"
ms.openlocfilehash: eb62dfce9f9507dd8806d91343cd39fe76e65594473683c1393d524f6c2d8a27
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893917"
---
# <a name="unable-to-activate-office"></a>Office를 정품 인증할 수 없습니다

**참고**: 이전 버전의 Windows(예: Windows 7)를 사용하는 경우 TLS 1.2가 기본값으로 사용하도록 설정되어 있는지 확인하세요. 자세한 내용은 [Windows의 WinHTTP에서 기본 보안 프로토콜로 TLS 1.1 및 TLS 1.2를 사용하도록 업데이트](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)를 참조하세요.

- 구독 상태가 만료되었는지 확인합니다.
- Office 365 Business 혹은 Business Premium과 같은 클라이언트 라이선스를 허용하는 구독이 있는지 확인하고 [사용자에게 라이선스가 할당되어 있는지 확인](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)합니다.
- 사용자가 라이선스가 할당된 동일한 계정으로 Office에 로그인하고 있는지 확인합니다.
- [Office 365 서비스 상태 페이지](https://docs.microsoft.com/office365/enterprise/view-service-health)를 보고 서비스에 알려진 문제가 있는지 확인합니다.
- 방화벽, 백신 소프트웨어 및 프록시 설정이 Microsoft 365 앱의 인터넷 액세스를 차단하고 있지 않은지 확인합니다. [Office 365 URL 및 IP 주소 범위](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL 및 IP 주소 범위")를 참조하세요.

**팁** Windows 컴퓨터에서 몇 가지 일반적인 Office 로그인 문제를 자동으로 진단하고 해결해드립니다. 자동화된 도구를 사용하려면 **[Office 365 지원 및 복구 도우미](https://aka.ms/SaRA-OfficeSignInScenario)** 를 다운로드하고 실행하십시오.

다음 정보를 사용하여 문제를 해결합니다.

- Office 앱을 열고 기존 사용자 계정을 [로그아웃](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)합니다. Office 라이선스를 [제거](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) 및 [다시 할당](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)한 다음 영향을 받는 사용자 계정을 사용하여 [Office에 로그인](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)합니다.
- [정품 인증 문제 해결사](https://aka.ms/SARA-OfficeActivation-Alchemy) 실행
- [Office 정품 인증 다시 설정](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Office 정품 인증 상태 재설정")
- [Office의 온라인 복구 실행](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

추가적인 문제 해결 솔루션을 보려면 다음을 참조하세요.  

- [사용 허가되지 않은 제품 및 Office 정품 인증 오류](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Office를 정품 인증할 때 "사용자 계정에 연결할 수 없습니다. 나중에 다시 시도해 보세요." 오류](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)