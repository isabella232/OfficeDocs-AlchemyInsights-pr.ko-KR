---
title: 기본 Yammer 도메인 변경
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
- "9002662"
- "5162"
ms.openlocfilehash: 93c82b7e60838e0127062e8bf5ab394bb29650d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793872"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>기본/주 Yammer 도메인 변경

Yammer URL은 Yammer 네트워크의 현재 주 도메인 이름을 포함합니다. 이 도메인 이름은 Office 365 또는 Azure AD에서 설정한 주 도메인 이름과 다를 수 있습니다. 테넌트에 추가된 사용자 지정 도메인의 수와 Yammer가 지원되는 구성(1개의 테넌트: 1개의 네트워크 또는 1:1) 상태에 따라 동작에 차이가 있습니다. [Yammer 도메인 및 Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains)에 대한 설명서를 사용할 수 있습니다.

잘못된 도메인이 표시되는 가장 일반적인 이유는 여러 Yammer 네트워크가 존재하고 있기 때문이며 이들은 통합되어야 합니다. 네트워크 마이그레이션 도구를 사용하여 [단일 네트워크로 통합](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)하는 것이 중요한 첫 단계입니다. 주 도메인을 설정하기 전에 이 작업을 완료하세요.

**사용자 지정이 되지 않은 도메인**

새 테넌트의 경우 테넌트의 기본 도메인(예: fabrikam.onmicrosoft.com)이 Yammer에 사용됩니다. 주 도메인이 yammer.com/fabrikam.onmicrosoft.com로 설정 됩니다.

**단일 사용자 지정 도메인**

Yammer는 Yammer의 주 도메인으로 테넌트에서 사용자 지정 도메인(예: fabrikam.com)을 자동으로 선택합니다. 이는 Yammer.com/fabrikam.com로 설정됩니다. 이 변경 사항은 도메인 동기화 서비스를 통해 적용되며 최대 24시간이 걸릴 수 있습니다.

**다수의 사용자 지정 도메인**

Yammer는 기본 테넌트 도메인과 다른 주 도메인을 가질 수 있습니다. 사용자 지정 도메인이 여러 개 있기 때문에 Yammer는 사용 가능한 도메인들 중에 올바른 도메인을 추측하려 시도하지 않습니다. 사용자는 원하는 주 도메인으로 주 도메인 이름을 변경하도록 요청하는 지원 사례를 열어야 합니다.

**추가 문제 해결 정보**

경우에 따라 테넌트 간에 도메인이 이동되어 도메인 동기화 서비스를 성공적으로 실행할 수 없었을 수도 있습니다. 사용자에게 잘못된 주 도메인 외에 로그인 또는 기타 문제가 발생할 수도 있습니다. 이 문제를 해결하기 위해 Microsoft 지원의 도움을 받아 도메인을 올바른 네트워크로 이동해야 할 수도 있습니다. 이러한 상황에서는 직접적인 도움이 필요하며, 문제를 해결하는데 시간이 다소 걸릴 수 있습니다(특히 도메인 이름 목록이 아주 긴 경우). 지원 사례를 열고 이러한 유형의 문제를 해결하는 데 도움을 받도록 합니다.

지원 에이전트를 이용하여 작업하는 경우, 도메인이 사용자의 제어 하에 테넌트에서 도메인이 확인되는지 검사를 진행할 것입니다. 에이전트는 테넌트에 추가되었지만 DNS에서 확인되지 않는 경우, 도메인에 대한 추가 확인 질문을 할 수도 있습니다. 도메인이 DNS에서 확인되는지 확인하여 프로세스의 속도를 높일 수 있도록 합니다..
