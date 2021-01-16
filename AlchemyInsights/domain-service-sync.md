---
title: 도메인 서비스 동기화
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876518"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="3f859-102">도메인 서비스 동기화</span><span class="sxs-lookup"><span data-stu-id="3f859-102">Domain service synchronization</span></span>

<span data-ttu-id="3f859-103">Azure AD DS(Azure Active Directory 도메인 서비스) 관리 도메인의 개체 및 자격 증명은 도메인 내에서 로컬로 만들거나 Azure AD(Azure Active Directory) 테넌트에서 동기화할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3f859-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="3f859-104">Azure AD DS를 처음 배포할 때 자동 단방형 동기화가 구성 및 시작하여 Azure AD에서 개체를 복제합니다.</span><span class="sxs-lookup"><span data-stu-id="3f859-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="3f859-105">이 단방형 동기화는 Azure AD의 변경 사항과 함께 Azure AD DS 관리 도메인을 최신으로 유지하기 위해 백그라운드에서 계속 실행됩니다.</span><span class="sxs-lookup"><span data-stu-id="3f859-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="3f859-106">Azure AD DS에서 Azure AD로 다시 동기화되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="3f859-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="3f859-107">Azure Active Directory 도메인 서비스 동기화에 대한 자세한 내용은 도메인 서비스 [동기화를 참조하세요.](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization)</span><span class="sxs-lookup"><span data-stu-id="3f859-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
