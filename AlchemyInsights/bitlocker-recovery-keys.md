---
title: Bitlocker 복구 키
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685892"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="d0851-102">Bitlocker 복구 키 액세스</span><span class="sxs-lookup"><span data-stu-id="d0851-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="d0851-103">Bitlocker 설정 Intune Endpoint Protection 정책을 구성할 때 Bitlocker 복구 정보를 Azure Active Directory에 저장할지 여부를 정의할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0851-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="d0851-104">이 설정이 구성 되어 있는 경우에는 다음과 같은 두 가지 방법으로 Intune 장치 블레이드에서 장치 레코드 데이터의 일부로 저장 된 복구 데이터를 Intune 관리자에 게 표시 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d0851-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="d0851-105">장치-Azure AD 장치-> "장치" 또는 장치-> 모든 장치-> "장치"-> 복구 키</span><span class="sxs-lookup"><span data-stu-id="d0851-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="d0851-106">또는 장치 자체에 대 한 관리 액세스 권한이 있는 경우 관리자 권한 명령 프롬프트에서 다음 명령을 실행 하 여 복구 키 (암호)를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0851-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="d0851-107">장치가 Intune에서 enrolment 전에 암호화 된 경우 복구 키가 OOBE 프로세스 중에 장치에 로그인 하는 데 사용 되는 "Microsoft 계정" (MSA)과 연결 되어 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0851-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="d0851-108">이 경우 해당 MSA에 액세스  https://onedrive.live.com/recoverykey 하 고 로그인 하려면 복구 키가 저장 된 장치가 표시 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d0851-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="d0851-109">장치가 도메인 기반 그룹 정책을 통해 구성 된 결과로 암호화 된 경우에는 온-프레미스 Active Directory에 복구 정보가 저장 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0851-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

