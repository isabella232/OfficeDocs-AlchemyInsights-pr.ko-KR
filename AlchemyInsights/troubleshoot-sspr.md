---
title: SSPR 문제 해결
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038964"
---
# <a name="troubleshoot-sspr"></a>SSPR 문제 해결

**암호 재설정을 구성하는 데 문제가 있습니다.**

- 셀프 서비스 암호 재설정을 사용하도록 설정하는 방법을 찾고 있는 경우 [자습서 SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)사용 을 참조하여 조직에 대한 암호 재설정을 구성합니다. 라이선스 요구 사항을 [검토할 수도 있습니다.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) 조직에 라이선스가 하나 이상 할당되어 있어야 합니다.
    - **클라우드 전용 사용자** - 모든 Office 365(O365) 유료 SKU 또는 Azure AD Basic
    - **클라우드 및/또는** 사내 사용자 - Azure AD Premium P1 P2, EMS(Enterprise Mobility + Security) 또는 SPE(Secure Productive Enterprise)
- 셀프 서비스 암호 재설정에 대한 자세한 질문은 [FAQ를 검토하세요.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**오류 메시지가 표시**

이 문서를 검토하여 일반적인 오류 및 해당 해결 방법 찾기: [셀프 서비스](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support) 암호 재설정 문제 해결

**암호 재설정 정책에 문제가 있습니다.**

- 암호 재설정 정책이 예상대로 행동하지 않는 경우 또는 암호 재설정 정책에 대한 질문이 있는 경우 다음 문서를 [검토하세요.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)Azure Active Directory.
- 암호 재설정 정책은 관리자에게 적용되지 않습니다. Microsoft는 Azure 관리자 역할에 대해 강력한 기본 2 게이트 암호 재설정 정책을 적용합니다. 관리자가 아닌 사용자와 테스트하는지 확인 관리자 재설정 정책에 대한 자세한 내용은 이 문서를 [참조하세요. 관리자](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)재설정 정책 차이점 .

**사용자가 암호 재설정을 위한 추가 보안 정보를 등록하지 못하게 하려는 경우**

API, PowerShell 또는 Azure AD 계정을 사용하여 사용자에 대한 데이터(전자 메일 및 전화 특성)를 미리 채우면 커넥트. 읽기 방법을 알아보는 방법:

- [사용자가 등록할 필요 없이 암호 재설정 배포](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [암호 재설정에 사용되는 데이터](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**사용자가 암호 재설정을 위한 추가 보안 정보를 등록할 수 있도록 하려는 경우**

1. 사용자가 셀프 서비스 암호 재설정에 대한 보안 정보를 등록할 수 있도록 에서 로 [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. 사용자 또는 관리자가 사용자에 대해 데이터를 채우고 나면 사용자가 [](https://passwordreset.microsoftonline.com/) 암호를 다시 aka.ms/sspr 권한을 부여할 수 있도록 사용자에게 지시합니다.
1. 사용자가 여전히 문제가 발생하는 경우 페더링 또는 암호 해시 동기화된 사용자일 가능성이 **높습니다.**  즉, 암호 쓰기 저장 서비스에 문제가 있을 수 있습니다.