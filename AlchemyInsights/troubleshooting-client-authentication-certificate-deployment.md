---
title: 클라이언트 인증 인증서 배포 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509071"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>클라이언트 인증 인증서 배포 문제 해결

Intune NDES/SCEP 및 PKCS/PFX 클라이언트 인증서 프로필은 사용자가 회사 리소스를 인증 하도록 허용하는 데 사용할 수 있는 Wifi, VPN, 전자 메일 등의 다른 프로필 유형과 함께 자주 사용됩니다. 해당 프로필 유형이 클라이언트 인증서 프로필에 연결되면, 해당 프로필 유형은 배포 성공 여부에 따라 달라집니다.

초기 인프라 설정과 클라이언트 인증서 프로필 관련 구성에는 종종 문제 해결이 필요합니다. NDES 커넥터의 성공적인 설정을 위한 단계별 가이드 및 인증서 배포에 관한 문제를 격리하는 문제 해결 지침은 다음을 참조하세요. 

- [Intune에서 SCEP를 지원하도록 인프라 구성](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Microsoft Intune에서 SCEP 인증서 프로필 문제 해결에 대한 개요](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

참조된 Powershell 스크립트로 구성을 확인해보세요. 자세한 내용은 [Intune 인증서 커넥터 확인 스크립트](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)를 참조하세요.

  
**기타 일반적인 문제**

**NDES 커넥터 서버에 Intune 인증서 커넥터를 설치하려고 하면 ‘인증서 요청의 암호를 확인할 수 없습니다. 이미 사용되었을 수 있습니다. 이 요청과 함께 제출할 새 암호를 가져옵니다.’라는 메시지가 표시 됩니다.**  

이 메시지는 사용자가 인증서 커넥터 설치를 관리자 권한으로 실행해야 함을 의미합니다.

일부 환경의 경우 Intune 인증서가 실행되는 서버에 프록시 서버를 사용하여 Intune에 연결해야 합니다. 따라서 인증서 커넥터에서 프록시를 사용해야 합니다. 경우에 따라 NDES 커넥터에서 구성된 프록시 설정을 무시하고 LocalSystem의 보안 컨텍스트를 실행하는 동안 프록시 설정을 구성해야 할 수 있습니다. 
 
Internet Explorer를 시스템으로 실행하고 IE에서 프록시를 구성하여 이 문제를 해결할 수 있습니다. Intune 커넥터 서비스를 다시 시작하면 NDES 커넥터가 Intune에 연결됩니다.

**사용자 장치의 경우에는 NDES에서 더 이상 SCEP 인증서를 받을 수 없습니다.**

NDES 서버에 발급되고 NDES 커넥터 설치 중에 지정된 클라이언트 인증 인증서가 만료되었거나 누락되었을 수 있습니다. 해결할 문제: 
 
1. NDES 커넥터를 제거합니다.  
2. 다음 세부 사항을 활용하여 새 클라이언트 인증 또는 서버 인증 인증서를 요청할 수 있습니다. 
 
    - 주체 이름: CN=외부 fqdn  
    - 주제 대체 이름(둘 다 필수): DNS=외부 fqdn, DNS=내부 fqdn 
 
3. 새 인증서를 사용하여 NDES 커넥터를 다시 설치합니다.