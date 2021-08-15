---
title: Azure AD 가입 장치에 대한 Single Sign-On 문제 해결
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
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039252"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Azure AD 가입 장치에 대한 Single Sign-On 문제 해결

사내 AD(Active Directory) 환경이 있는 경우 AD 도메인에 가입된 컴퓨터를 Azure AD에 가입하려는 경우 하이브리드 Azure AD 조인을 수행하여 이 작업을 수행할 수 있습니다. [방법: 하이브리드 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 조인 구현을 계획하면 사용자 환경에서 하이브리드 Azure AD 조인을 구현하는 관련 단계를 제공합니다.

자세한 내용은 [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business을 참조하십시오.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**PRT(기본 새로 고침 토큰) 문제**

PRT(주 새로 고침 토큰)는 Windows 10, Windows Server 2016 버전, iOS 및 Android 장치에서 Azure AD 인증의 주요 아티팩트입니다. Microsoft 자사 토큰 브로커에 특수하게 발급된 JWT(JSON Web Token)으로, 이러한 장치에서 사용되는 응용 프로그램에서 SSO(Single Sign-On)를 사용하도록 설정할 수 있습니다. Windows 10 장치에서 PRT를 발급, 사용 및 보호하는 방법에 대한 자세한 내용은 주 새로 고침 [토큰이란?을 참조하세요.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

**WamDefaultSet: YES 및 AzureADPrt: YES**

이러한 필드는 사용자가 디바이스에 로그인할 때 Azure AD에 인증을 완료한 것인지 여부를 나타냅니다. 값이 **NO이면** 다음 때문일 수 있습니다.

- 등록 시 장치와 연결된 TPM의 잘못된 저장소 키(상승된 실행 시 KeySignTest 확인)
- 대체 로그인 ID
- HTTP 프록시를 찾을 수 없습니다.

dsregcmd 명령을 사용하여 디바이스 문제를 해결 방법은 [SSO 상태를 참조합니다.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
