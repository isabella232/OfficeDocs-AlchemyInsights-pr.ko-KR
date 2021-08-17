---
title: '도메인 컨트롤러 '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: b044e69cef177c5a1ad38c2d27a297d90ba7f55e7b2e75fff2e390869241f325
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057900"
---
# <a name="domain-controller"></a>도메인 컨트롤러

**AAD-DS를 사용할 수 없거나 배포가 실패하는 경우**

AAD-DS(Azure AD 도메인 서비스)가 활성화되지 않거나 배포되지 않는 문제를 해결하려면 다음 단계를 수행합니다.

1. 이미 존재하는 가상 네트워크를 사용하는 경우 포털(https://aka.ms/aadds-networking)의 AAD-DS에서 동기화하는 데 필요한 포트를 차단하는 규칙이 있는지 NSG를 확인하세요.
2. https://aka.ms/aadds-troubleshoot-enable확인하세요
3. 새 가상 네트워크에 Azure AD 도메인 서비스를 배포합니다.
4. [Azure AD Domain Services 생성 지침서](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)에서 제공하는 AAD-DS를 배포하는 방법에 대한 시작 가이드를 따르세요.
5. Azure AD Domain Services 배포에 문제가 있는 경우 [Azure AD 도메인 서비스 문제 해결](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)을 참조하여 일반적인 오류를 해결하여 작업을 다시 시작할 수 있습니다. 

**AAD-DS를 사용하지 않도록 설정할 수 없음**

AAD-DS를 일시 중지할 수 없습니다. 관리 도메인 사용을 중지하려면 삭제해야 합니다.

문제가 발생하면 일반적인 오류 메시지를 해결하고 작업을 다시 실행하는 데 도움이 되는 관련 문제 해결 단계는 [Azure Active Directory Domain Services 문제 해결](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)을 참조하세요.
