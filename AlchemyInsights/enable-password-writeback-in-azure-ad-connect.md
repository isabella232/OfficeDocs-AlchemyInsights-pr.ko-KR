---
title: Azure AD Connect에서 암호 쓰기 저장 사용
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709733"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Azure AD Connect에서 암호 쓰기 저장 사용

셀프 서비스 암호 재설정 쓰기 저장을 사용하려면 Azure AD Connect에서 쓰기 저장 옵션을 먼저 설정합니다. Azure AD Connect 서버에서 다음 단계를 완료합니다.

1. Azure AD Connect 서버에 로그인하고 **Azure AD Connect** 구성 마법사를 시작합니다.
2. **시작** 페이지에서 **구성**을 클릭합니다.
3. **추가 작업** 페이지에서 **동기화 옵션 사용자 지정**을 선택한 다음 **다음**을 클릭합니다.
4. **Azure AD에 연결** 페이지에서 Azure 테넌트에 대한 전역 관리자 자격 증명을 입력한 후 다음을 클릭합니다.
5. **디렉터리 연결** 및 **도메인/OU** 필터링 페이지에서 **다음**을 클릭합니다.
6. **선택적 기능** 페이지에서 **암호 쓰기 저장** 옆에 있는 상자를 선택하고 **다음**을 클릭합니다.
7. **구성 준비** 페이지에서 **구성**을 클릭하고 프로세스가 완료될 때까지 기다립니다.
8. 구성이 완료되면 **종료**를 클릭합니다.

Azure AD Connect에서 암호 쓰기 저장이 사용하도록 설정되어 있는 경우 쓰기 저장용 Azure AD SSPR를 구성합니다.  SSPR에서 암호 쓰기 저장을 사용하려면 다음 단계를 완료합니다.

1. 전역 관리자 계정을 사용하여 Azure Portal 포털에 로그인합니다.
2. **Azure Active Directory**를 검색하고 선택하여 **암호 재설정**을 클릭한 다음 **온-프레미스 통합**을 선택합니다.
3. **온-프레미스 디렉터리에 암호를 쓰기 저장하시겠습니까?** 옵션을 **예**로 설정합니다.
4. **사용자가 암호를 재설정하지 않고 계정을 잠금 해제할 수 있도록 하시겠습니까?** 옵션을 **예**로 설정합니다.
5. 준비되면 **저장**을 클릭합니다.

자세한 내용은 [온-프레미스 환경에서 Azure Active Directory 셀프 서비스 암호 재설정 쓰기 저장 사용](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)을 참조하세요.
