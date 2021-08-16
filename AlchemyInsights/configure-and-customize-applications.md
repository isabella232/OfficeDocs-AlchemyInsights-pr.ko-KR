---
title: 응용 프로그램 구성 및 사용자 지정
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004334"
- "7733"
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044994"
---
# <a name="configure-and-customize-applications"></a>응용 프로그램 구성 및 사용자 지정

**응용 프로그램 구성**

1. [빠른 시작: Azure Active Directory(Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) 테넌트의 응용 프로그램에 대한 속성을 구성하면 앱의 일부 속성을 구성하는 방법을 보여 주게 됩니다.
2. 응용 프로그램과 응용 프로그램을 Azure Active Directory 구성을 진행하는 자습서 컬렉션을 개발했습니다. [](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)
3. [응용 프로그램 프록시 응용](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) 프로그램을 구성하는 방법을 통해 Azure AD 내에서 응용 프로그램 프록시 응용 프로그램을 구성하여 클라우드에 프레미스 응용 프로그램을 노출하는 방법을 이해할 수 있습니다.
4. [PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)다운로드 및 응용 프로그램 구성: *Configure PingAccess for Azure AD의* 지침에 따라 Ping Identity 웹 사이트에서 Microsoft Azure AD 응용 프로그램 프록시를 사용하여 게시된 응용 프로그램을 보호하고 최신 버전의 PingAccess를 다운로드합니다.

**잘못 구성된 응용 프로그램(AADSTS650056) 오류**

1. 응용 프로그램 소유자가 제공한 로그인 주소에서 응용 프로그램에 액세스하는지 확인 그렇지 않으면 일반 프로세스를 통해 응용 프로그램에 로그인합니다. 대부분의 경우 이는 자동으로 해결됩니다. 그렇지 않은 경우 이 게시물은 문제 해결 및 해결에 도움이 될 수 있습니다.
2. **조직에서 응용 프로그램을 소유하는 경우(응용** 프로그램 등록이 조직에 있는 경우)
    - 최소한 Microsoft 365의 위임된 사용 권한을 추가하는 Graph `User.Read` `openid` 좋습니다. 
    - 응용 프로그램 및 모든 사용 권한이 동의하는지 확인 API 사용 권한 내에서  응용 프로그램 등록의 상태 열을 확인하여 **이를 확인할 수 있습니다.**
    - 일부 시나리오에서는 응용 프로그램이 타사일 수 있습니다. 그러나 조직에 등록될 수 있습니다. 이 응용 프로그램이 앱 등록에 나열되어 Enterprise 않습니다.
    - 이 오류 메시지가 계속 표시될 경우 그런 다음 4단계에 설명된 동의 URL을 **작성해야 할 수 있습니다.**
3. **조직이 응용 프로그램 소유자가** 아니며 이를 타사 응용 프로그램으로 사용하는 경우:
    - 전역/회사 관리자인 경우 동의 화면이 표시됩니다. "조직을 대신하여 **동의"** 확인란을 선택해야 합니다.
    - If you don't see the consent screen, delete the Enterprise application, and try again.
    - 이 오류 메시지가 계속 표시될 경우 그런 다음 4단계에 설명된 동의 URL을 **작성해야 할 수 있습니다.**
4. 사용할 동의 URL을 수동으로 작성: 응용 프로그램이 특정 리소스에 액세스하도록 디자인된 경우 Azure Portal에서 동의 단추를 사용하지 못하게 될 수 있습니다. 직접 동의 **URL을** 수동으로 생성하고 이 URL을 사용해야 합니다.
    - 응용 프로그램 소유자로부터 `{App-Id}` 및 `{App-Uri-Id}` 를 얻게 됩니다. `{Tenant-Id}` 는 테넌트 식별자입니다. 이 ID는 또는 `yourdomain.onmicrosoft.com` 디렉터리 ID입니다.
    - 응용 프로그램이 리소스에 대해 자체 액세스하는 경우 `{App-Id}` 및 `{App-Uri-Id}` 는 동일합니다.
5. 자세한 내용은 SAML 기반 Single Sign-On 구성된 앱에 로그인하는 문제를 [참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**응용 프로그램 사용자 지정**

- [조직의 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) 로그인 페이지에 브랜드 추가 - 조직의 로고 및 사용자 지정 색 구성표를 사용하여 Azure AD(Azure Active Directory 로그인 페이지에 일관된 모양과 느낌을 제공합니다.
- [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) 포털을 사용하여 사용자 지정 도메인 이름을 추가합니다. 모든 새 Azure AD 테넌트에는 초기 도메인 이름이 함께 표시됩니다. 초기 도메인 이름을 변경하거나 삭제할 수 없지만 조직의 이름을 추가할 수 있습니다. 사용자 지정 도메인 이름을 추가하면 사용자에게 친숙한 사용자 이름을 만들 수 있습니다.
