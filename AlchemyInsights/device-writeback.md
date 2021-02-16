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
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255172"
---
# <a name="device-writeback"></a>장치 쓰기백

장치 쓰기 기록은 다음과 같은 시나리오에서 사용됩니다.

- 하이브리드 인증서 신뢰 배포를 사용하여 비즈니스용 [Windows Hello 사용](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- ADFS(2012 R2 이상) 보호된 응용 프로그램(신뢰하는 사용자 트러스트)에 대한 장치에 기반한 조건부 액세스 사용

    > [!NOTE]
    > 디바이스 쓰기 저장소를 위해 Azure AD Premium 구독이 필요합니다.

이렇게 하면 응용 프로그램에 대한 액세스가 신뢰할 수 있는 디바이스에만 부여됩니다. 조건부 액세스에 대한 자세한 [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) 내용은 조건부 액세스로 위험 관리 및 Azure Active Directory 장치 등록을 사용하여 [On-premises 조건부 액세스를 설정하는 방법을 참조하세요.](https://docs.microsoft.com/azure/active-directory/devices/overview)

장치에 대해 장치 쓰기 기록을 사용하도록 설정하는 데 대한 자세한 내용은 장치 쓰기 기록 [사용을 참조하세요.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
