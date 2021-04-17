---
title: ConsistencyGuid/sourceAnchor 동작
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816998"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor 동작

Azure AD Connect(버전 1.1.524.0 이상)를 사용하면 msDS-ConsistencyGuid를 sourceAnchor 특성으로 쉽게 사용할 수 있습니다. 이 기능을 사용하는 경우 Azure AD Connect는 동기화 규칙을 다음으로 자동으로 구성합니다.
  
- User 개체의 sourceAnchor 특성으로 msDS-ConsistencyGuid를 사용합니다. ObjectGUID는 다른 개체 형식에 사용됩니다.
    
- msDS-ConsistencyGuid 특성이 채워지지 않은 주어진 모든 사내 AD User 개체의 경우 Azure AD Connect는 해당 objectGUID 값을 다시 On-premises Active Directory의 msDS-ConsistencyGuid 특성에 기록합니다. msDS-ConsistencyGuid 특성이 채워진 후 Azure AD Connect는 개체를 Azure AD로 내보낼 수 있습니다.
    
 **참고:** Azure AD Connect로 가져온(즉, AD 커넥터 공간으로 가져와 메타버스로 투영된) On-프레미스 AD 개체를 가져온 후 더 이상 sourceAnchor 값을 변경할 수 없습니다. 지정한 사내 AD 개체에 대한 sourceAnchor 값을 지정하기 위해 Azure AD Connect로 가져오기 전에 해당 msDS-ConsistencyGuid 특성을 구성합니다. 
  
SourceAnchor 및 ConsistencyGuid에 대한 자세한 내용은 [Azure AD Connect: 디자인 개념을 참조하세요.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

