---
title: Bitlocker 복구 키
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820292"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Bitlocker 복구 키 액세스

Bitlocker 설정 Intune 끝점 보호 정책을 구성할 때 Bitlocker 복구 정보를 Azure Active Directory에 저장할지 여부를 정의할 수 있습니다.

해당 설정이 구성된 경우 저장된 복구 데이터는 Intune 장치 블레이드의 장치 레코드 데이터의 일부로 Intune 관리자에게 다음 두 가지 방법으로 표시해야 합니다.

장치 - Azure AD 장치 -> "장치" 또는 장치 -> 모든 장치 -> "장치" -> 복구 키

또는 장치 자체에 대한 관리 액세스 권한이 있는 경우 관리자 권한 명령 프롬프트에서 다음 명령을 실행하여 복구 키(암호)를 볼 수 있습니다.

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Intune에 등록하기 전에 장치가 암호화된 경우 복구 키가 OOBE 프로세스 중에 장치에 로그인하는 데 사용되는 "Microsoft 계정"(MSA)과 연결되어 있을 수 있습니다. 이 경우 해당 MSA를 사용하여 액세스하고 로그인하면 복구 키가 저장된  https://onedrive.live.com/recoverykey 디바이스가 표시될 수 있습니다.
 
도메인 기반 그룹 정책을 통해 구성한 결과로 장치가 암호화된 경우 복구 정보가 사내 Active Directory에 저장될 수 있습니다.

Azure Active Directory에 복구 키를 저장하도록 끝점 보호 정책을 구성했지만 특정 장치의 키가 업로드되지 않은 경우 MEM 콘솔에서 해당 장치에 대한 복구 키를 회전하여 업로드를 트리거할 수 있습니다. 자세한 내용은 [BitLocker 복구 키 회전을 참조합니다.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

