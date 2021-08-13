---
title: SCP(서비스 연결 지점 구성)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 5ccb55996ccef4b55c8d80de6e35f4ba27e3dfa18dfcaeaf6f6ad1c54b6bb376
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965971"
---
# <a name="configure-service-connection-point-scp"></a>SCP(서비스 연결 지점 구성)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **이유**: SCP 개체를 읽고 Azure AD 테넌트 정보를 얻을 수 없습니다.
- **해결**: [서비스 연결 지점 구성](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join) 섹션을 참고하세요.


**실행 계획**

- 장치가 제어된 유효성 검사에 대한 GPO를 받았는지 확인합니다.
- GPO에서 레지스트리 키를 만들었는지 확인합니다.
- 디렉터리 ID와 onmicrosoft 도메인으로 키 2개가 만들어졌다는 것을 확인합니다.

**SCP에 대한 클라이언트 레지스트리 설정 구성**

다음 예제를 사용하여 GPO(그룹 정책 개체)를 만들어 장치의 레지스트리에서 SCP 항목을 구성하는 레지스트리 설정을 배포합니다.

1. 그룹 정책 관리 콘솔을 열고 도메인에 새 GPO를 만듭니다.
     - 새로 만든 GPO의 이름(예: ClientSideSCP)을 입력합니다.

2. GPO를 편집하고 다음 경로를 찾습니다. **컴퓨터 구성 > 기본 설정 > Windows 설정 > 레지스트리**.

3. **레지스트리** 에 오른쪽 클릭하고 **신규 > 레지스트리 항목** 을 선택합니다.

4. **일반** 탭에서 다음을 구성합니다.
  
- **작업**: 업데이트
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **키 경로**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **값 이름**: TenantId
    
- **값 형식**: REG_SZ
    
- **값 데이터**: Azure AD 인스턴스의 GUID 또는 디렉터리 ID(이 값은 **Azure Portal > Azure Active Directory > 속성 > 디렉터리 ID**)에서 찾을 수 있음)
 
- **확인** 을 클릭합니다.
 
5. **레지스트리** 에 오른쪽 클릭하고 **신규 > 레지스트리 항목** 을 선택합니다.

6. **일반** 탭에서 다음을 구성합니다.
  
- **작업**: 업데이트
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **키 경로**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **값 이름**: TenantName
    
- **값 형식**: REG_SZ
    
- **값 데이터**: AD FS와 같은 페더레이션된 환경을 사용하는 경우 확인된 도메인 이름입니다. 관리되는 환경을 사용하는 경우 확인된 도메인 이름 또는 onmicrosoft.com 도메인 이름(예: contoso.onmicrosoft)입니다.

- **확인** 을 클릭합니다.

7. 새로 만든 GPO의 편집기를 닫습니다.

8. 제어된 출시 인구에 속하는 도메인에 가입된 컴퓨터를 포함하여 원하는 OU에 새로 만든 GPO를 연결합니다.

자세한 내용은  [하이브리드 Azure AD 제어 유효성 검사 참가 - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) 및  [하이브리드 Azure Active Directory에 가입된 장치 문제해결 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)을 확인하세요.









