---
title: 장치 쓰기백
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
- "9003257"
- "8279"
ms.openlocfilehash: c069d0b4588e53250d6cc1f3a66c744ea5c12ae4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320092"
---
# <a name="device-writeback"></a>장치 쓰기백

장치 쓰기백은 다음과 같은 시나리오에서 사용됩니다.

- 하이브리드 [Windows Hello 트러스트 배포를 사용하여 비즈니스용 인증 사용](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- ADFS(2012 R2 이상) 보호된 응용 프로그램(신뢰하는 사용자 트러스트)에 대한 장치에 기반한 조건부 액세스 사용

    **참고:** 디바이스 쓰기 Azure AD Premium 구독이 필요합니다.

이렇게 하면 응용 프로그램에 대한 액세스가 신뢰할 수 있는 디바이스에만 부여되는 추가 보안 및 보장이 보장됩니다. 조건부 액세스에 대한 자세한 내용은 [조건부](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) 액세스로 위험 관리 및 장치 등록을 사용하여 Azure Active Directory [설정을 참조하세요.](https://docs.microsoft.com/azure/active-directory/devices/overview)

장치에 대해 장치 쓰기 기록을 사용하도록 설정하는 데 대한 자세한 내용은 [Enable Device Writeback을 참조하십시오.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
