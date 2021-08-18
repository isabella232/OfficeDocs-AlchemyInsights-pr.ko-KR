---
title: 도메인에 가입된 장치를 사용하여 조건부 액세스에서 차단되는 경우
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: d71bb376615191f507d39b99d9e51ca77d929b90
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323444"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>도메인에 가입된 장치를 사용하여 조건부 액세스에서 차단되는 경우

**권장 도구**

[장치 등록 문제 도구](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - 가장 일반적인 장치 등록 문제를 해결하는 데 도움이 되는 도구입니다.

[장치 등록 연결 스크립트 테스트](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - 장치가 시스템 계정 아래에 있는 장치 등록 끝점에 액세스할 수 있는지를 확인하는 데 도움이 되는 스크립트입니다.

[Azure AD 장치 정리 스크립트](https://github.com/mzmaili/AzureADDeviceCleanup) - 환경에서 오래된 장치를 검색하고 관리할 수 있는 스크립트입니다.

다음은 도메인(하이브리드 Azure AD)에 가입된 장치에서 조건부 액세스에 실패하는 몇 가지 일반적인 이유입니다.

1. **장치에 Azure AD PRT가 없음** - 장치에 Azure AD 기본 새로 고침 토큰(PRT)이 있어야 합니다. PRT에 대한 자세한 내용은 이 [문서](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)를 참조하세요.

Azure AD PRT가 있는지 확인하려면 장치에서 `dsregcmd/status` 명령을 실행하고 "AzureAdPrt"가 "YES"인지 확인할 수 있습니다.

"AzureAdPrt"가 "NO"인 경우 다음을 검사합니다.

- **AD FS 페더레이션 환경이 있으며 사용자의 홈 네트워크에서 액세스할 수 없는 경우**: 이 경우 엑스트라넷에서 "usernamemixed" 끝점에 액세스할 수 있는지 확인합니다. AD FS가 VPN를 통해 제공되는 경우 사용자는 VPN에 연결하고 장치에 다시 로그인해야 합니다. 자세한 정보는 이 [문서](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)를 참조하세요.

- **장치의 TPM에 문제가 있어 장치를 인증할 수 없는 경우**: "tpm.msc"를 확인하여 TPM 상태가 "Ready"인지 확인합니다. 그렇지 않은 경우 `dsregcmd/leave`를 실행하고 장치가 Azure AD에 다시 참가하게 합니다. 그런 후에 다시 시도합니다. 자세한 정보는 이 [문서](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)를 참조하세요.

- **WS-Trust 프로토콜을 지원하지 않는 제3자 ID 공급자를 사용하고 있습니다**. 문서에 설명된 대로 이 경우 하이브리드 Azure AD에 가입된 장치에서는 작동할 수 없습니다. ID 공급자에게 지원을 요청하세요.

2. **사용자가 Windows 10 계정 없이 Chrome을 사용** 하거나 **Office 확장 Chrome에서 AAD에 가입 또는 하이브리드 AAD에 가입된 장치의 PRT를 자동으로 사용되지 않은 경우**: 이 경우 장치 기반 조건부 액세스 정책에 실패하게 되며 "등록되지 않은 장치" 오류 메시지가 표시됩니다. Chrome 브라우저를 올바르게 사용하려면 SCCM 또는 Intune을 통해 "Windows 10 계정" 또는 "사용자의 Chrome 브라우저로 Office 확장"을 설치해야 합니다. 자세한 정보는 이 [문서](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)를 참조하세요.

원격으로 확장을 푸시할 수 없는 경우 사용자에게 위 확장 중 하나를 수동으로 설치하여 장치 기반 조건부 액세스의 기반이 되는 응용 프로그램에 액세스하도록 알립니다. 자세한 정보는 이 [문서](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)를 참조하세요.

3. **장치가 올바르게 하이브리드 Azure AD에 조인됐지만, Azure AD Connect 또는 Azure Portal의 동기화 변경 사항으로 인해 장치가 우연히 삭제되거나 비활성화된 경우**: 이 경우 장치에서 "AzureAdJoined" 및 "PRT" 상태가 유효한 것으로 표시되어도 장치 개체가 더 이상 완전히 가입된 장치로 인식되지 않습니다.

이 문제를 해결하기 위해 영향을 받는 장치에서 `dsregcmd/leave`을(를) 실행한 다음 Azure AD에 다시 연결합니다. 자세한 내용은 이 [문서](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)를 참조하세요.

**참고**: 장치가 Windows 10, 1809 업데이트이며 VPN/클라우드 프록시를 사용하고 "AzureAdPrt" 상태와 관련된 문제가 표시되거나 앱에 SSO 문제(PRT가 있음에도 Outlook이 사서함에 연결되지 않음)가 있는 경우 이번 패치 [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) 또는 4월 누적 업데이트 [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6)를 통해 해당 컴퓨터에 PRT 오류를 방지하세요.

















