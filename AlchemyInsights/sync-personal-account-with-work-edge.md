---
title: 사용자가 Microsoft Edge에서 회사 계정과 개인 계정을 동기화할 수 있도록 설정
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: 627048f21eb931188dfebd3f4177be2bbd65c71e26ab2d0e302f5ab49e9fbc53
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900078"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>사용자가 Microsoft Edge에서 회사 계정과 개인 계정을 동기화할 수 있도록 설정

다음 기준을 충족하는지 확인하세요.

- 엔터프라이즈 상태 로밍은 Azure Active Directory 관리 센터에서 활성화되며 Azure Active Directory Premium 또는 EMS(Enterprise Mobility + Security)에 대한 구독이 필요합니다. 자세한 내용은 [Azure Active Directory에서 엔터프라이즈 상태 로밍 활성화](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-enable)를 참조하세요.
- 다음 기준 중 하나 또는 모두가 충족됩니다.
    - 테넌트에 대해 Azure Information Protection 서비스가 사용하도록 설정되어 있습니다. 자세한 내용은 [Microsoft 365 관리 센터에서 Azure Rights Management 보호 사용](https://docs.microsoft.com/azure/information-protection/activate-office365)을 참조하세요.
    - Azure Active Directory ESR(Enterprise State Roaming) 기능은 모든 사용자 또는 테넌트에 대해 사용하도록 설정됩니다. 자세한 내용은 [엔터프라이즈 상태 로밍이란 무엇입니까?](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-overview)를 참조하세요.

AIP와 ESR이 모두 비활성화된 경우 오류 메시지는 사용자에게 계정에 대해 동기화를 사용할 수 없음을 알려줍니다.
