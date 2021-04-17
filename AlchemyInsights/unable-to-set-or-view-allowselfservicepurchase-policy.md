---
title: AllowSelfServicePurchase 정책을 설정하거나 볼 수 없습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826097"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="9d9d5-102">AllowSelfServicePurchase 정책을 설정하거나 볼 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="9d9d5-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="9d9d5-103">AllowSelfServicePurchase 정책을 설정하거나 확인하려고 하면 다음 오류 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="9d9d5-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="9d9d5-104">*HandleError : PolicyId 'AllowSelfServicePurchase', ErrorMessage를 사용하여 제품 정책을 검색하지 못했습니다. - 연결이 닫혔습니다. 보내기 시 예기치 않은 오류가 발생했습니다.*</span><span class="sxs-lookup"><span data-stu-id="9d9d5-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="9d9d5-105">이전 버전의 TLS(전송 계층 보안) 때문일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d9d5-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="9d9d5-106">MSCommerce 서비스를 연결하려면 TLS 1.2 이상을 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9d9d5-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="9d9d5-107">다음 단계를 수행하여 TLS 프로토콜을 1.2로 설정하고 확인한 후 다시 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="9d9d5-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="9d9d5-108">PowerShell 명령 프롬프트(PS C: 다음 명령을 입력하여 TLS 프로토콜을 버전 \) 1.2로 설정)</span><span class="sxs-lookup"><span data-stu-id="9d9d5-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="9d9d5-109">다음 명령을 사용하여 사용 중인 TLS 프로토콜을 검증합니다.</span><span class="sxs-lookup"><span data-stu-id="9d9d5-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="9d9d5-110">필요한 경우 Get 또는 Update 명령을 다시 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="9d9d5-110">Retry the Get or Update commands as needed.</span></span>

