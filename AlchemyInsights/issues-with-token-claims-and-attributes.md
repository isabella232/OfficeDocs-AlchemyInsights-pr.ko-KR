---
title: 토큰 클레임 및 특성 관련 문제
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50029989"
---
# <a name="issues-with-token-claims-and-attributes"></a>토큰 클레임 및 특성 관련 문제

**토큰 클레임 업데이트, 구성 또는 제거**

1. Azure AD(Azure Active Directory)를 사용하면 앱에 권한을 승인한 후 받은 응답 토큰에서 역할 클레임에 대한 클레임 유형을 사용자 지정할 수 있습니다. [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)
2. 응용 프로그램 개발자는 Azure AD 응용 프로그램에서 선택적 클레임을 사용하여 응용 프로그램으로 전송되는 토큰에서 원하는 클레임을 지정할 수 있습니다. 자세한 내용은 앱에 [대한 선택적 클레임 제공을 참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. Azure Active Directory를 사용하여 응용 프로그램에 [대한 그룹 클레임 구성](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. 응용 프로그램에서 Seamless Single Sign-On을 사용하는 경우 엔터프라이즈 응용 프로그램에 대한 SAML 토큰에서 발급된 클레임 사용자 [지정을 참조합니다.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**클레임 특성 매핑**

1. PowerShell을 사용하여 클레임 매핑 정책을 구성하기 위해 테넌트의 특정 앱에 대한 토큰으로 내보인 클레임 사용자 지정(미리 보기)을 [참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. 디렉터리 Schema 확장 특성은 사용자 개체 및 기타 디렉터리 개체(예: 그룹, 테넌트 세부 정보, 서비스 주체)에 Azure Active Directory에 추가 데이터를 저장할 수 있는 방법을 제공합니다. 응용 프로그램에 클레임이 표시될 때 사용자 개체의 확장 특성만 사용할 수 있습니다. [클레임에서 디렉터리 schema 확장](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) 특성을 사용하여 토큰 클레임의 응용 프로그램으로 사용자 데이터를 전송하는 데 디렉터리 schema 확장 특성을 사용하는 방법을 설명합니다.

토큰 클레임에 대한 자세한 내용은 다음을 참조하세요.

- [액세스 토큰의 클레임](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [클레임의 id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) Azure AD B2C에서 발급한 ID 토큰 및 액세스 토큰에서 기대할 수 있는 클레임
- [SAML 토큰 클레임 참조](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
