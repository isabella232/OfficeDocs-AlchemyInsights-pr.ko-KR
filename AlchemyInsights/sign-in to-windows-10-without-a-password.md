---
title: 암호를 사용 하지 않고 Windows 10에 로그인
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719959"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>암호를 사용 하지 않고 Windows 10에 로그인

Windows 시작 시 암호를 입력 하지 않으려면 PIN, 얼굴 인식 또는 지문 같은 Windows Hello 보안 로그인 옵션 중 하나를 사용 하는 것이 좋습니다 (사용 가능한 경우). 보안 로그인을 실제로 사용 하지 않으려면 아래의 "Windows 10에 자동으로 로그인" 지침을 참조 하세요.

**계정 암호 대신 Windows Hello 보안 대안을 적용할 수 있습니다.**

**로그인 옵션 > 설정 > 계정** 으로 이동 하거나 [여기](ms-settings:signinoptions?activationSource=GetHelp)를 클릭 합니다. 사용 가능한 로그인 옵션이 나열 됩니다. 예시:

![로그인 옵션](media/sign-in-options.png)

옵션 중 하나를 클릭 하거나 탭 하 여 구성 합니다. 다음 번에 Windows를 시작 하거나 잠금 해제할 때 암호 대신 새로 만들기 옵션을 사용할 수 있습니다. 

**자동으로 Windows 10에 로그인**

**참고**: 자동 로그인은 편리 하지만, 특히 PC가 여러 사용자가 액세스할 수 있는 경우에는 보안 위험을 야기 합니다. 

1. 작업 표시줄에서 **시작** 단추를 클릭 하거나 탭 합니다.

2. **Netplwiz** 를 입력 하 고 Enter 키를 눌러 사용자 계정 창을 엽니다.

3. **사용자 계정**에서 Windows가 시작 될 때 자동으로 로그인 할 계정을 클릭 합니다.

4. "사용자가이 컴퓨터를 사용할 수 있는 사용자 이름과 암호를 입력 해야 합니다." 확인란의 선택을 취소 합니다.

    ![사용자가 사용자 이름 및 암호를 입력 해야 합니다.](media/users-must-enter-username.png)

5. **확인**을 클릭합니다. 선택한 계정에 대 한 암호를 입력 하 고 확인 하 라는 메시지가 표시 됩니다. **확인**을 클릭하여 작업을 마칩니다. 다음 번에 Windows 10을 시작 하면 선택한 계정에 자동으로 로그인 됩니다.
