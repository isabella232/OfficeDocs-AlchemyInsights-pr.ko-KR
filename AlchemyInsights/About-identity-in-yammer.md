---
title: Yammer의 ID 정보
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664176"
---
# <a name="about-identity-in-yammer"></a>Yammer의 ID 정보

ID 관련 문제가 발생 하지 않도록 하려면 모든 네트워크에 다음 단계를 수행하는 것이 좋습니다.

1. 모든 사용자가 기본 Microsoft 365 계정을 사용하여 로그인 하도록 Azure AD의 사용자에 대해 Microsoft 365 계정을 프로비전 한 후 Office 365 ID를 적용하세요. 자세한 내용은 [Yammer 사용자에 Office 365 ID 적용](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)을 참조하세요.
2. 여러 Yammer 네트워크 통합 레거시 Yammer 구성에서는 여러 Yammer 네트워크를 하나의 테넌트로 연결할 수 있습니다. 자세한 내용은 [네트워크 마이그레이션: 여러 Yammer 네트워크 통합](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)을 참조하세요.
3. Yammer 라이선스가 없는 사용자를 차단하기 위하여 Yammer 라이선스를 강제할 수 있는 옵션이 있습니다. 자세한 내용은 [Office 365에서 Yammer 사용자 라이선스 관리](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)를 참조하세요.
4. 마지막으로, 이전 Yammer 네트워크의 사용자 목록을 감사하고 레거시 사용자를 일시 중단 합니다. 삭제를 취소할 수 없으므로 사용자를 삭제하는 대신 일시 중단 (비활성화)을 하는 것이 좋습니다. 자세한 내용은 [Office 365에 연결된 네트워크에서 Yammer 사용자를 감사](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) 및 [사용자 삭제](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)를 참조하세요.

이 단계를 사용하여 Yammer를 구성하면 Microsoft 365의 기본 모드에서 Yammer 네트워크를 구성 할 수 있습니다. 자세한 내용은 [Microsoft 365 기본 모드 Yammer 네트워크 구성](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)을 참조하세요.