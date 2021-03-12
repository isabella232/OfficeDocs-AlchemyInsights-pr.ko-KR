---
title: DKIM에 대한 사용자 지정 도메인 사용
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 1a21101602f47dcb5c9b607d7bbccfacec00f43a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736754"
---
# <a name="enable-the-custom-domain-for-dkim"></a><span data-ttu-id="11a37-102">DKIM에 대한 사용자 지정 도메인 사용</span><span class="sxs-lookup"><span data-stu-id="11a37-102">Enable the custom domain for DKIM</span></span>

<span data-ttu-id="11a37-103">사용자 지정 도메인에 대한 CNAME 레코드를 만든 후 도메인을 사용하도록 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="11a37-103">After you create the CNAME records for your custom domains, you need to enable the domain.</span></span>

<span data-ttu-id="11a37-104">도메인을 사용하도록 설정하려면 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="11a37-104">To enable the domain, perform the following steps:</span></span>

1. <span data-ttu-id="11a37-105">Exchange 관리 [센터로 이동합니다.](https://outlook.office365.com/ecp/)</span><span class="sxs-lookup"><span data-stu-id="11a37-105">Navigate to the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>
2. <span data-ttu-id="11a37-106">왼쪽 창에서 **dkim 에서 보호 > 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="11a37-106">In the left pane, select **protection > dkim**.</span></span>
3. <span data-ttu-id="11a37-107">도메인을 선택한 다음 **DKIM** 서명을 사용하여 이 도메인에 대한 메시지 서명에서 사용 을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="11a37-107">Select the domain, and then under **Sign messages for this domain with DKIM signatures**, click **Enable**.</span></span> <span data-ttu-id="11a37-108">각 도메인에 대해 이 단계를 반복합니다.</span><span class="sxs-lookup"><span data-stu-id="11a37-108">Repeat this step for each domain.</span></span>

