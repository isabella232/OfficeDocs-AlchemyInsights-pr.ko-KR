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
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="25d93-102">ConsistencyGuid/sourceAnchor 동작</span><span class="sxs-lookup"><span data-stu-id="25d93-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="25d93-103">Azure AD Connect(버전 1.1.524.0 이상)를 사용하면 msDS-ConsistencyGuid를 sourceAnchor 특성으로 쉽게 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25d93-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="25d93-104">이 기능을 사용하는 경우 Azure AD Connect는 동기화 규칙을 다음으로 자동으로 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="25d93-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="25d93-105">User 개체의 sourceAnchor 특성으로 msDS-ConsistencyGuid를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="25d93-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="25d93-106">ObjectGUID는 다른 개체 형식에 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="25d93-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="25d93-107">msDS-ConsistencyGuid 특성이 채워지지 않은 주어진 모든 사내 AD User 개체의 경우 Azure AD Connect는 해당 objectGUID 값을 다시 On-premises Active Directory의 msDS-ConsistencyGuid 특성에 기록합니다.</span><span class="sxs-lookup"><span data-stu-id="25d93-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="25d93-108">msDS-ConsistencyGuid 특성이 채워진 후 Azure AD Connect는 개체를 Azure AD로 내보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25d93-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="25d93-109">**참고:** Azure AD Connect로 가져온(즉, AD 커넥터 공간으로 가져와 메타버스로 투영된) On-프레미스 AD 개체를 가져온 후 더 이상 sourceAnchor 값을 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="25d93-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="25d93-110">지정한 사내 AD 개체에 대한 sourceAnchor 값을 지정하기 위해 Azure AD Connect로 가져오기 전에 해당 msDS-ConsistencyGuid 특성을 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="25d93-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="25d93-111">SourceAnchor 및 ConsistencyGuid에 대한 자세한 내용은 [Azure AD Connect: 디자인 개념을 참조하세요.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="25d93-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

