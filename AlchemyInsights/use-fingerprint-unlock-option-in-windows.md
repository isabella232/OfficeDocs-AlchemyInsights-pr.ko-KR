---
title: Windows 10에서 지문 잠금 해제 옵션 사용
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795250"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Windows 10에서 지문 잠금 해제 옵션 사용

**Windows Hello 지문 사용**

지문을 사용 하 여 Windows 10의 잠금을 해제 하려면 windows Hello 지문을 추가 하 고 (Windows에서 인식할 수 있도록 허용) 하나 이상의 손가락을 설치 해야 합니다. 

1. **로그인 옵션 > 설정 > 계정** 으로 이동 하거나 [여기](ms-settings:signinoptions?activationSource=GetHelp)를 클릭 합니다. 사용 가능한 로그인 옵션이 나열 됩니다. 예시:

    ![로그인 옵션](media/sign-in-options.png)

2. **Windows Hello 지문을**클릭 하거나 탭 한 다음 **설정을**클릭 합니다. Windows Hello 설정 창에서 **시작**을 클릭 합니다. 지문 센서가 정품 인증 되며 손가락을 센서에 배치 하 라는 메시지가 표시 됩니다.

   ![지문 센서입니다.](media/fingerprint-sensor.png)

3. 손가락을 반복적으로 검사 하는 지침을 따릅니다. 이 작업이 완료 되 면 로그인에 사용할 다른 손가락을 추가할 수 있는 옵션이 표시 됩니다. 다음 번에 Windows 10에 로그인 할 때 지문을 사용 하 여이 작업을 수행할 수 있습니다.

**로그인 옵션으로 Windows Hello 지문을 사용할 수 없음**

**로그인 옵션**에서 Windows Hello 지문이 옵션으로 표시 되지 않는 경우 WINDOWS는 pc에 연결 된 지문 판독기/스캐너를 인식 하지 않거나 시스템 정책에 따라 사용을 차단 하는 경우 (예를 들어, PC가 회사에서 관리 하는 경우)에는 사용할 수 없습니다. 해결 방법: 

1. 작업 표시줄에서 **시작** 단추를 선택 하 고 **장치 관리자**를 검색 합니다.

2. **장치 관리자**를 클릭 하거나 탭 하 여 엽니다.

3. 장치 관리자에서 해당 갈매기형 펼침 단추를 클릭 하 여 생체 인식 장치를 확장 합니다.

   ![생체 인식 장치](media/biometric-devices.png)

4. 지문 스캐너가 Synaptics WBDI 스캐너와 같은 생체 인식 장치로 나열 되어야 합니다.

   ![생체 인식 장치](media/biometric-devices-expanded.png)

5. 지문 스캐너가 표시 되지 않고 스캐너가 PC에 통합 되어 있는 경우 PC 제조업체의 웹 사이트로 이동 합니다. PC 모델의 기술 지원 섹션에서 설치할 수 있는 스캐너용 Windows 10 드라이버를 검색 합니다.

6. 스캐너가 PC와 별개인 경우 (USB를 통해 연결 됨) 스캐너 제조업체의 웹 사이트로 이동 하 여 검색 프로그램 모델에 대 한 Windows 10 장치 드라이버 소프트웨어를 찾아서 설치 합니다.
