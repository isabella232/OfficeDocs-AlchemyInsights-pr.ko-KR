---
title: 암호 동기화
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960841"
---
# <a name="password-synchronization"></a>암호 동기화

**암호 해시 동기화가 작동하지 않습니다.**

암호 해시 동기화가 작동하지 않을 때 고객에게 발생하는 몇 가지 일반적인 문제는 같습니다.

- Azure AD 커넥트 Active Directory와 통신하는 데 사용하는 Active Directory 계정에는  암호 동기화에  필요한 모든 복제 디렉터리 변경 및 복제 디렉터리 변경 권한이 부여되지 않습니다. Active Directory 계정에 이러한 사용 권한을 부여하여 이 문제를 해결해야 합니다.
- 암호 해시 동기화는 관리자가 사용자 Sign-In 메서드를 암호 동기화에서 Azure AD 커넥트 마법사에서 **AD FS와의** 페더링과 같은 다른 옵션으로 변경한 후에  사용하지 않도록 설정됩니다. Azure AD 커넥트 마법사에서 암호 해시 동기화 기능을 다시 사용하도록 설정하면 이 문제를 해결할 수 있습니다. 
- 프레미스 Active Directory의 연결 문제입니다. 예를 들어 일부 도메인 컨트롤러는 Azure AD 커넥트 액세스할 [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) 수 없는 경우 또는 필요한 포트가 방화벽에 의해 차단됩니다. Azure AD 커넥트 서버와 프레미스 Active Directory 간의 연결이 올바르게 작동하는지 확인하여 이 문제를 해결해야 합니다.
- Azure AD 커넥트 현재 준비 모드에 있는 서버로 인해 서버가 암호 해시를 사용할 수 없습니다. 문제를 해결하기 위해 [Azure AD](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)커넥트 동기화와 암호 동기화 문제 해결 - 암호가 동기화되지 않습니다. 섹션에 설명된 단계를 따르세요.

**일부 사용자에 대해 암호 해시 동기화가 작동하지 않습니다.**

1. 사용자에 대해 암호 해시가 동기화되지 않는 경우  Azure AD 2013의 문제 해결 작업을 사용하여 문제를 커넥트 해결합니다. 다음 작업을 수행합니다.

    a. [마법사에서 문제 해결 작업 실행](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [문제 해결 cmdlet을 사용하여 특정 사용에 대한 암호 해시 동기화 문제 조사](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. 사용자에 대해 사용할 수 있는 On-premises Active Directory User 개체는 다음 로그온 시 암호를 **변경해야** 합니다. 이 옵션을 사용하도록 설정하면 사용자에게 임시 암호가 할당되어 다음 로그온 시 암호를 변경하라는 메시지가 표시됩니다. Azure AD 커넥트 Azure AD와 임시 암호를 동기화하지 않습니다.

위의 문제를 해결하기 위해 다음 작업 중 하나를 수행합니다.

- 사용자에게 데스크톱과 같은 사내 응용 프로그램에 Windows 암호를 변경하도록 요청합니다. 새 암호가 Azure AD와 동기화됩니다.
- 관리자가 다음 로그온할 때 암호를 변경해야 합니다. 옵션을 사용하도록 설정하지 않고 사용자의 암호를 업데이트하도록 합니다. **및** 새 암호를 사용자와 공유합니다.

3. 개체 동기화 또는 암호 동기화를  위해 On-premises Active Directory User 개체가 올바르게 구성되지 않았습니다. 이 문제를 해결하기 위해 Azure [AD와](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)암호 해시 동기화 문제 해결에 설명된 단계를 커넥트 수행합니다.







