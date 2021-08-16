---
title: AAD 도메인 서비스를 통한 가상 구성
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 03a6ec63ba8e2779b0fe3f0381606af2c0748f8b848baaa7cd88b61317bd7a5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072850"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>AAD 도메인 서비스를 통한 가상 구성

AAD 도메인 서비스를 통한 가상 구성에는 다음 단계가 필요합니다. 

1. Azure Portal(https://aka.ms/aadds-health)에서 도메인 상태를 확인합니다.
2. NSG에서 포털(https://aka.ms/aadds-networking)의 Azure AD Domain Services에서 동기화하는 데 필요한 포트를 차단하는 규칙을 확인합니다.
3. 가상 네트워크가 Azure AD Domain Services 관리 도메인과 동일한 Azure 영역에 배포되었는지 확인합니다.
4. 가상 네트워크에서 사용할 수 있는 동일한 도메인 이름이 있는 기존 도메인이 없는지 확인합니다.

AAD 도메인 서비스를 지원하기 위한 Azure Virtual Network의 설계 고려사항에 대한 자세한 내용은 [가상 네트워크 고려 사항](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)을 참조하세요.

