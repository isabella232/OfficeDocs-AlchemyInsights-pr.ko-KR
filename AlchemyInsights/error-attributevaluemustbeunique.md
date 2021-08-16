---
title: Error AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002126"
---
# <a name="error-attributevaluemustbeunique"></a>오류: AttributeValueMustBeUnique

AttributeValueMustBeUnique 오류의 가장 일반적인 이유는 SourceAnchor(immutableId)가 서로 다른 두 개체의 ProxyAddresses 및/또는 UserPrincipalName 특성 값이 같기 때문에 발생합니다. AttributeValueMustBeUnique 오류를 해결합니다.
  
1. 중복된 proxyAddresses, userPrincipalName 또는 오류를 일으키는 기타 특성 값을 식별합니다. 또한 충돌과 관련된 두 개 이상의 개체도 식별합니다. 동기화를 위해 Azure AD 커넥트 생성하는 보고서는 두 개체를 식별하는 데 도움이 될 수 있습니다.
    
2. 중복된 값을 계속 사용할 개체와 중복되지 않을 개체를 식별합니다.
    
3. 해당 값이 없는 개체에서 중복된 값을 제거합니다. 개체를 원본으로 하는 디렉터리에서 변경해야 합니다. 경우에 따라 충돌하는 개체 중 하나를 삭제해야 할 수 있습니다.
    
4. If you made the change in the on premises AD, let Azure AD 커넥트 sync the change for the error to get fixed.
    

