---
title: 오류 AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709157"
---
# <a name="error-attributevaluemustbeunique"></a>오류: AttributeValueMustBeUnique

AttributeValueMustBeUnique 오류가 발생 하는 가장 일반적인 원인은 ProxyAddresses 및/또는 UserPrincipalName 특성에 대해 다른 SourceAnchor (immutableId)의 값이 같은 개체 두 개를 사용 하는 것입니다. AttributeValueMustBeUnique 오류를 해결 하려면
  
1. 중복 되는 proxyAddresses, userPrincipalName 또는 기타 특성 값을 식별 하 여 오류를 발생 시킵니다. 또한 충돌에 관여 하는 두 개 이상의 개체를 식별 합니다. 동기화를 위해 Azure AD Connect Health에서 생성 한 보고서는 두 개체를 식별 하는 데 도움이 될 수 있습니다.
    
2. 계속 해 서 복제 되는 값과 사용할 수 없어야 하는 개체를 식별 합니다.
    
3. 해당 값이 없어야 하는 개체에서 중복 된 값을 제거 합니다. 개체를 원본으로 하는 디렉터리에서 변경 작업을 수행 해야 합니다. 경우에 따라 충돌이 발생 하는 개체 중 하나를 삭제 해야 할 수 있습니다.
    
4. 온-프레미스 AD에서 변경을 수행한 경우 Azure AD Connect에서 오류에 대 한 변경 사항을 동기화 하 여 수정 합니다.
    

