---
title: Single-Sign 가입된 장치에 Azure Active Directory 사용
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050016"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>가입된 디바이스에 Azure Active Directory Single Sign-On

사내 AD(Active Directory) 환경이 있는 경우 AD 도메인에 가입된 컴퓨터를 Azure AD에 가입하려는 경우 하이브리드 Azure AD 조인을 수행하여 이 작업을 수행할 수 있습니다. [방법: 하이브리드 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 조인 구현을 계획하면 사용자 환경에서 하이브리드 Azure AD 조인을 구현하는 관련 단계를 제공합니다.

[비즈니스용 디바이스를 사용하여 Single-Sign Azure AD 가입 Windows Hello 구성](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**PRT(기본 새로 고침 토큰) 문제** PRT(주 새로 고침 토큰)는 Windows 10, Windows Server 2016 버전, iOS 및 Android 장치에서 Azure AD 인증의 주요 아티팩트입니다. Microsoft 자사 토큰 브로커에 특수하게 발급된 JWT(JSON Web Token)으로, 이러한 장치에서 사용되는 응용 프로그램에서 SSO(Single Sign-On)를 사용하도록 설정할 수 있습니다. [기본 새로 고침 토큰이란?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)에서 PRT를 발급, 사용 및 보호하는 방법에 대한 세부 정보를 Windows 10 있습니다.

**WamDefaultSet: YES 및 AzureADPrt: YES** 이러한 필드는 사용자가 디바이스에 로그인할 때 Azure AD에 인증을 완료한 것인지 여부를 나타냅니다. 값이 **NO인** 경우 다음이 때문일 수 있습니다.

- 등록 시 장치와 연결된 TPM의 잘못된 저장소 키입니다(상승된 실행 시 KeySignTest 확인).
- 대체 로그인 ID
- HTTP 프록시를 찾을 수 없습니다.

dsregcmd 명령 - [SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state) 상태를 사용하여 장치 문제 해결
