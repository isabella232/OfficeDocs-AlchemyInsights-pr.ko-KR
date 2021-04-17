---
title: 암호를 사용하지 않고 Windows 10에 로그인
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830552"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>암호를 사용하지 않고 Windows 10에 로그인

Windows 시작 시 암호를 입력할 필요 없이 PIN, 얼굴 인식 또는 지문(사용 가능한 경우)과 같은 Windows Hello 보안 로그인 옵션 중 하나를 사용하는 것이 좋습니다. 보안 로그인을 사용하지 않도록 설정하려는 경우 아래 "Windows 10에 자동으로 로그인" 지침을 참조하세요.

**계정 암호 대신 Windows Hello 보안**

설정 > 계정 > **로그인 옵션으로** 이동합니다(또는 여기를 [클릭하십시오).](ms-settings:signinoptions?activationSource=GetHelp) 사용 가능한 로그인 옵션이 나열됩니다. 예시:

![로그인 옵션.](media/sign-in-options.png)

옵션 중 하나를 클릭하거나 탭하여 구성합니다. 다음에 Windows를 시작하거나 잠금을 해제하면 암호 대신 새 옵션을 사용할 수 있습니다. 

**Windows 10에 자동으로 로그인**

**참고:** 자동 로그인은 편리하지만 특히 여러 사용자가 PC에 액세스할 수 있는 경우 보안 위험이 있습니다. 

1. 작업 표시줄에서 **시작** 단추를 클릭하거나 탭합니다.

2. **netplwiz를** 입력하고 Enter 키를 입력하여 사용자 계정 창을 여십시오.

3. 사용자 **계정에서** Windows가 시작될 때 자동으로 로그인하려는 계정을 클릭합니다.

4. "사용자가 이 컴퓨터를 사용하려면 사용자 이름과 암호를 입력해야 합니다." 확인란의 선택을 선택하지 않습니다.

    ![사용자는 사용자 이름 및 암호 옵션을 입력해야 합니다.](media/users-must-enter-username.png)

5. **확인** 을 클릭합니다. 선택한 계정의 암호를 입력하고 확인해야 합니다. **확인** 을 클릭하여 작업을 마칩니다. 다음에 Windows 10이 시작되면 선택한 계정에 자동으로 로그인합니다.
