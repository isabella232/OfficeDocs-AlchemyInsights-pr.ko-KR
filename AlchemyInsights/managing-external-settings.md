---
title: 외부 설정 관리
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50282834"
---
# <a name="managing-external-settings"></a>외부 설정 관리

**알림**

- [2021년 1월 4일부터 Google의 WebView 로그인 지원을 중단합니다](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support). 호환성 테스트에 대한 Google의 지침을 따라 앱이 영향을 받는지 테스트합니다.
- 소비자 Google 계정으로 사용자를 로그인할 때 시스템 웹 보기 또는 시스템 브라우저를 사용해야 합니다.

**초대 설정 관리**

적절한 사용자가 초대를 보낼 수 있도록 [외부 공동 작업 설정을 구성했는지](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) 확인합니다.

**게스트 사용자 액세스 권한 관리**

1. 전역 관리자는 외부 공동 작업 설정 페이지에서 게스트 액세스 권한을 구성하여 Azure Portal을 통해 디렉터리의 게스트 액세스 권한을 관리할 수 있습니다. [이 설정에 대해 자세히 알아보세요](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).
2. 게스트가 Teams 또는 SharePoint와 같은 앱에 액세스하도록 하려면 게스트 액세스를 허용하도록 해당 앱을 구성했는지 확인합니다. [Teams 설정](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) 및 [Sharepoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)에 대해 자세히 알아보세요.

**초대 구성:**

- [B2B 외부 공동 작업을 활성화하고 게스트를 초대할 수 있는 사용자 관리](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [특정 조직의 사용자에 대한 초대 허용 또는 차단](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

**허용된 ID 공급자 구성:**

- [Google 페더레이션](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [직접 페더레이션](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [전자 메일 일회용 암호 인증](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
