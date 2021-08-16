---
title: 규격 장치를 사용하여 조건부 액세스에서 차단되는 경우
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019154"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>규격 장치를 사용하여 조건부 액세스에서 차단되는 경우

**권장 도구**

- [장치 등록 문제 도구](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - 가장 일반적인 장치 등록 문제를 해결하는 데 도움이 되는 포괄적인 도구입니다.
- [장치 등록 연결 스크립트 테스트](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - 장치가 시스템 계정 아래에 있는 장치 등록 끝점에 액세스할 수 있는지를 확인하는 데 사용되는 도구입니다.
- [Azure AD 장치 정리 스크립트](https://github.com/mzmaili/AzureADDeviceCleanup) - 환경에서 오래된 장치를 검색하고 관리하는 데 사용되는 도구입니다.

다음은 규격 장치에 대한 조건부 액세스가 실패하는 일반적인 이유 또는 조직 리소스에 대한 로그인 요청 중에 사용자가 **여기서는 연결할 수 없습니다** 메시지를 수신하는 몇 가지 일반적인 이유입니다.

1. **장치가 MDM과 함께 필요한 장치 상태가 아닌 경우**:

장치가 Intune과 같은 승인된 MDM 제공자에 등록되어 있고 *준수* 로 표시되어 있는지 확인합니다. Intune에 대한 Intune자세한 내용은 이 [문서](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)를 확인하세요. 장치 규정 준수 및 Intune에 대한 자세한 내용은 [규정 준수 정책을 사용하여 Intune으로 관리하는 장치에 대한 규칙을 설정](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)을 참조하세요. 장치를 Intune으로 등록하는 데 문제가 있는 경우 [Microsoft의 장치 등록 문제 해결](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)에서 문제 해결 세부 정보를 찾습니다. Intune 지원에 대한 지원 요청은 지원 요청을 작성하세요. 지원 요청을 작성하려면 [Intune 도움말 및 지원 페이지](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)를 방문하세요.

2. **장치가 조직 네트워크에 연결되어 있지 않은 경우**:

조직 리소스에 액세스하려면 장치를 직접 연결 또는 VPN(가상 사설망)을 통해 조직의 네트워크에 연결하고 온-프레미스 또는 Azure Active Directory에도 연결해야 합니다. 조직 장치를 조직 네트워크에 연결하려면 [조직 장치를 조직 네트워크에 연결](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network)을 참조하세요. 개인/BYOD 장치를 등록하려면 [개인 장치를 조직 네트워크에 연결](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)을 참조하세요.

- 장치가 네트워크에 연결되어 있는지 확인하려면 단계에 따라 [여기](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered)에서 등록된 장치를 확인하거나 [여기](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined)에서 작동 중인 장치를 확인하세요. 조직 네트워크 연결 문제를 범위 지정하려면 다음 지침을 따르세요.

    1. 회사 또는 학교 계정(예: alain@contoso.com)을 사용하여 Windows에 로그인합니다.
    2. VPN이나 DirectAccess를 통해 조직 네트워크에 연결합니다.
    3. 연결한 후, **Windows 로고 키 + L** 을 눌러 장치를 잠급니다.
    4. 회사 또는 학교 계정을 사용하여 장치를 잠금 해제하고 문제가 있는 앱이나 서비스에 다시 액세스합니다.

**여기서는 불가능합니다** 오류 메시지가 다시 표시되면, 다른 곳에서 문제가 발생할 수도 있습니다.

3. **운영 체제가 지원되지 않는 경우**:

다음을 포함한 지원되는 버전에서 실행 중인지 확인합니다.

- **Windows 클라이언트**: Windows 7 또는 이상

- **Windows Server**: Windows Server 2008 R2 또는 이상

- **macOS**: macOS X 또는 이상

- **Android 및 iOS**: 최신 버전의 Android 및 iOS 모바일 운영 체제

4. **지원되지 않는 웹 브라우저의 경우**:

아래에서 지원되는 브라우저를 찾아 보세요. Windows 1703 이상 버전에서 Chrome을 지원하려면 Windows 10 계정 확장이 필요합니다. Edge 85 이상의 경우 장치 규정 준수 정보를 제대로 전달하려면 사용자가 로그인해야 합니다. 자세한 내용은 [여기](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)를 참조하세요.

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune 관리되는 브라우저, Safari
- **Android**: **Microsoft Edge**: Intune 관리되는 브라우저, Chrome
- **Windows 휴대폰**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

**여기에서는 불가능합니다** 에 대한 자세한 내용은 메시지와 [여기](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)의 문제 해결 단계를 참조하세요.
