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
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884583"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="8ecce-102">AAD 도메인 서비스를 통한 가상 구성</span><span class="sxs-lookup"><span data-stu-id="8ecce-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="8ecce-103">AAD 도메인 서비스를 통한 가상 구성에는 다음 단계가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="8ecce-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="8ecce-104">Azure Portal(https://aka.ms/aadds-health)에서 도메인 상태를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="8ecce-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="8ecce-105">NSG에서 포털(https://aka.ms/aadds-networking)의 Azure AD Domain Services에서 동기화하는 데 필요한 포트를 차단하는 규칙을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="8ecce-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="8ecce-106">가상 네트워크가 Azure AD Domain Services 관리 도메인과 동일한 Azure 영역에 배포되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="8ecce-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="8ecce-107">가상 네트워크에서 사용할 수 있는 동일한 도메인 이름이 있는 기존 도메인이 없는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="8ecce-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="8ecce-108">AAD 도메인 서비스를 지원하기 위한 Azure Virtual Network의 설계 고려사항에 대한 자세한 내용은 [가상 네트워크 고려 사항](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8ecce-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

