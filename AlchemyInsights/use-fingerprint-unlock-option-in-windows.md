---
title: 지문 잠금 해제 옵션 Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971941"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>지문 잠금 해제 옵션 Windows 10

**지문 Windows Hello 사용**

지문을 Windows 10 잠금을 해제하려면 하나 이상의 손가락을 Windows Hello 추가하여 Windows 지문을 설정해야 합니다. 

1. 로그인 **설정 > 계정 >** (또는 여기를 [클릭)로 이동하세요.](ms-settings:signinoptions?activationSource=GetHelp) 사용 가능한 로그인 옵션이 나열됩니다. 예제:

    ![로그인 옵션.](media/sign-in-options.png)

2. 지문을 **Windows Hello 클릭하거나** 탭한 다음 **설정 을 클릭합니다.** 설치 Windows Hello **시작을 클릭합니다.** 지문 센서가 활성화됩니다. 센서에 손가락을 대어 두는 것이 요청됩니다.

   ![지문 센서입니다.](media/fingerprint-sensor.png)

3. 지침에 따라 손가락을 반복적으로 스캔할 것을 요청합니다. 이 완료되면 로그인에 사용할 수 있는 다른 손가락을 추가할 수 있습니다. 다음에 로그인하면 Windows 10 지문을 사용하여 로그인할 수 있습니다.

**Windows Hello 로그인 옵션으로 사용할 수 없는 지문**

Windows Hello 지문이 로그인 옵션에 옵션으로 표시되어 있지 않은 경우 Windows PC에 연결된 지문 판독기/스캐너를 인식하지 못하거나 시스템 정책이 사용을 차단하는 것입니다(예: PC가 작업 공간에서 관리하는 경우).  문제 해결: 

1. 작업 **표시줄에서** 시작 단추를 선택하고 장치 **관리자를 검색합니다.**

2. 장치 관리자를 클릭하거나 **탭하여 를 니다.**

3. 장치 관리자에서 확장형을 클릭하여 생체 인식 장치를 확장합니다.

   ![생체 인식 장치.](media/biometric-devices.png)

4. 지문 스캐너는 Synaptics WBDI 스캐너와 같은 생체 인식 장치로 나열해야 합니다.

   ![생체 인식 장치.](media/biometric-devices-expanded.png)

5. 지문 스캐너가 표시되어 있지 않고 스캐너가 PC에 통합되어 있는 경우 PC 제조업체의 웹 사이트로 이동하세요. PC 모델에 대한 기술 지원 섹션에서 설치할 수 있는 Windows 10 드라이버를 검색합니다.

6. 스캐너가 PC와 별개인 경우(USB를 통해 연결) 스캐너 제조업체의 웹 사이트로 이동하여 Windows 10 모델에 대한 장치 드라이버 소프트웨어를 찾아서 설치합니다.
