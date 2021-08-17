---
title: SAML 서명 인증서 문제 해결
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 290e740ccd7f3beac5b77e63c32c5b18c295070e6002dcdde44ce4a93f4330f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105682"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>SAML 서명 인증서 문제 해결

SAML 서명 인증서 문제를 해결하려면 다음 권장 단계를 수행하세요.

1. SSO를 지원하는 엔터프라이즈 애플리케이션을 추가할 경우 Azure가 [SAML 서명 인증서](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)라는 인증서를 생성합니다. 이 인증서의 유효기간은 3년입니다. 인증서 만료 날짜를 변경하려면 [페더레이션 인증서의 만료 날짜를 사용자 지정하고 새 인증서에 롤오버](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)를 참조하세요.
2. Azure는 이 인증서를 사용하여 응용 프로그램에서 요청한 SAML 토큰에 서명하고 성공적인 SSO를 위해 이 토큰을 응용 프로그램으로 전송합니다. 이 작업을 완료하려면 Azure 포털에서 인증서를 다운로드한 후 애플리케이션 공급업체로 전송하여 SSO 프로세스를 완료하세요.

이 프로세스가 완료되면 응용 프로그램이 이 인증서를 신뢰하고 이 인증서로 서명된 모든 SAML 토큰이 응용 프로그램에서 승인됩니다.

3. 이 인증서가 만료되면 새 인증서를 만들고 응용 프로그램 공급업체로 업데이트한 다음 Azure 측에서 활성화하세요. 자세한 내용은 [곧 만료되는 인증서 갱신](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)을 참조하세요.

> [!NOTE]
> 인증서가 만료될 경우, 사용자는 차단되지 않습니다.

4. 현재 인증서가 만료되기 전에 수신될 [알림에 대한 전자 메일 주소를 추가](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration)합니다.

> [!NOTE]
> 4단계는 선택 사항입니다.

5. 응용 프로그램의 SAML 인증서 서명 옵션 및 인증서 서명 알고리즘을 변경합니다. 자세한 내용은 [인증서 서명 옵션 및 서명 알고리즘 변경](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)을 참조하세요.

