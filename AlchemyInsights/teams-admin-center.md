---
title: Teams 관리 센터
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049350"
---
# <a name="teams-admin-center"></a>Teams 관리 센터

[Teams 관리 센터](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center)를 이용하여 Teams를 관리하는 방법을 알아봅니다.

Teams 관리 센터에 액세스할 수 없는 경우, 다음 항목을 확인하세요.

- 모든 주변 장치(방화벽 등) 혹은 로컬 컴퓨터의 방화벽 규칙에 적절한 [Office 365 IP 주소와 URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service)을 허용했는지 확인합니다.
- Teams 관리 포털에 액세스하는 데 사용 중인 로그인이 [Microsoft 365 관리 포털](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)에 나열된 사용자 이름과 일치하는지 확인합니다.

Teams 관리 센터에 사용자가 나타나지 않는 경우, 다음 항목을 확인하세요.

- 최근 24시간 동안 사용자를 만들었거나 라이선스를 할당했나요? 반드시 지원 티켓을 열기 전 최소한 24시간을 기다립니다.
- 적절한 라이선스를 할당했는지 확인합니다.
- 온-프레미스 Active Directory를 가지고 있다면, [현지 Active Directory에 있는 ProxyAddresses 필드의 msRTCSIP-PrimaryUserAddress 또는 SIP 주소값이 고유하고, 형식이](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) [Microsoft 365 관리 센터](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)의 사용자 sip:**Username** 과 일치하는지 확인하세요.
- 비즈니스용 Skype 서버 배포를 유지하고 사용자가 온-프레미스와 온라인에 속하도록 하려면, 비즈니스용 Skype 서버 제어판에서 **"Teams와 비즈니스용 Skype 온라인을 하이브리드로 설정"** 을 참고하고 사용자를 온라인으로 이동하세요.
