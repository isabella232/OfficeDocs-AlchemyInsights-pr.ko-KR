---
title: AD FS 배포
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
- "1300012"
- "7420"
ms.openlocfilehash: c4059364cd8aba920dba833c88a69413bad95a2c3b895599d9f6895b50ff73d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079636"
---
# <a name="deploy-ad-fs"></a>AD FS 배포

AD FS(Active Directory Federation Services) 배포는 사내 인프라를 사용하여 Office 365 서비스를 인증합니다. 페더타 로그인을 사용하면 사용자가 Azure AD(Office 365)와 통합된 SAAS(Software as a Service) 응용 프로그램에 로그인할 수 Azure Active Directory 있습니다. 페더러드 로그인은 AD FS를 통해 사용자의 On-premises Active Directory에 대해 사용자를 인증합니다. 또한 회사 네트워크에 있는 동안에는 사용자가 암호를 다시 입력할 필요는 없습니다.

AD FS 배포 [고문은](https://go.microsoft.com/fwlink/?linkid=2071178) Microsoft 365 및 Office 365 서비스를 인증하는 사내 AD FS 인프라 배포에 대한 단계별 지침을 제공합니다. 이 가이드를 사용하여 조직은 AD FS 구성 요소 및 요구 사항을 검토하고, 배포에 필요한 SSL 인증서를 획득 및 설치하고, 필요한 웹 응용 프로그램 프록시 서버를 설치할 수 있습니다.
