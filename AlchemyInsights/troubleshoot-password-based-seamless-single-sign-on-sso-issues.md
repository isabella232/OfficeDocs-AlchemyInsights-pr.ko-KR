---
title: 암호 기반 원활한 SSO(Single Sign-On) 문제 해결
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972830"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>암호 기반 원활한 SSO(Single Sign-On) 문제 해결

암호 기반 SSO의 기본에 대한 자세한 내용은 에서 암호 [기반 인증을 Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**암호 기반 SSO 구성**

1. [암호 기반 Single Sign-On](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) 구성 - 이 문서에서는 암호 기반 SSO 옵션에 대해 자세히 설명하고 있습니다. 추가할 응용 프로그램에 사용자 지정 구성이 필요하고 암호 기반 SSO를 사용해야 하는 경우 이 문서가 도움이 됩니다.
2. [프레미스 앱에](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) 대한 암호 기반 Single Sign-On 구성 - 응용 프로그램 프록시는 몇 가지 Single Sign-On 모드를 지원합니다. 암호 기반 로그인은 인증에 사용자 이름/암호 조합을 사용하는 응용 프로그램을 위한 것입니다. 응용 프로그램에 대해 암호 기반 로그인을 구성할 때 사용자는 한 번만 On-premises 응용 프로그램에 로그인해야 합니다. 그런 Azure Active Directory 로그인 정보를 저장하고 사용자가 원격으로 액세스할 때 응용 프로그램에 자동으로 제공합니다.
    - 응용 프로그램 프록시를 사용하여 앱을 게시하고 테스트해야 합니다. 그렇지 않은 경우 [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) 응용 프로그램 프록시를 사용하여 응용 프로그램 게시의 단계를 따라 프레미스 앱에 대한 암호 기반 SSO 구성을 계속합니다.

암호 기반 SSO 문제 해결을 위해 Azure AD에서 암호 기반 [Single Sign-On 문제 해결을 참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
