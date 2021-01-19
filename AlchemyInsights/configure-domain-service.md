---
title: 도메인 서비스 구성
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884620"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="d2b5f-102">AAD-DS를 활성화할 수 없거나 배포할 수 없는 경우</span><span class="sxs-lookup"><span data-stu-id="d2b5f-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="d2b5f-103">AAD-DS(Azure AD 도메인 서비스)가 활성화되지 않거나 배포되지 않는 문제를 해결하려면 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="d2b5f-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="d2b5f-104">이미 존재하는 가상 네트워크를 사용하는 경우 포털(https://aka.ms/aadds-networking)의 AAD-DS에서 동기화하는 데 필요한 포트를 차단하는 규칙이 있는지 NSG를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="d2b5f-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="d2b5f-105"> https://aka.ms/aadds-troubleshoot-enable확인하세요</span><span class="sxs-lookup"><span data-stu-id="d2b5f-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="d2b5f-106">새 가상 네트워크에 Azure AD 도메인 서비스를 배포합니다.</span><span class="sxs-lookup"><span data-stu-id="d2b5f-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="d2b5f-107">AAD-DS를 배포하는 방법에 대한 시작 가이드 [AAD Domain Services 만들기 및 구성](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="d2b5f-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="d2b5f-108">Azure AD Domain Services 배포에 문제가 있는 경우 [Azure AD 도메인 서비스 문제 해결](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)을 참조하여 일반적인 오류를 해결하여 작업을 다시 시작할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d2b5f-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="d2b5f-109">**AAD-DS를 사용하지 않도록 설정할 수 없음**</span><span class="sxs-lookup"><span data-stu-id="d2b5f-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="d2b5f-110">AAD-DS를 일시 중지할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="d2b5f-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="d2b5f-111">관리 도메인 사용을 중지하려면 삭제해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d2b5f-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="d2b5f-112">관리 도메인을 삭제하려면 [AAD Domain Service 삭제](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d2b5f-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



