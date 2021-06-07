---
title: Microsoft 365 Import Service의 드라이브 배송
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721723"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="b747f-102">Microsoft 365 Import Service의 드라이브 배송</span><span class="sxs-lookup"><span data-stu-id="b747f-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="b747f-103">하드 드라이브에 PST를 복사한 다음 하드 드라이브를 Microsoft로 배송하여 드라이브 배송을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="b747f-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="b747f-104">작업을 시작하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="b747f-104">To start the job:</span></span>

1. <span data-ttu-id="b747f-105">Microsoft 365 준수 센터의 **정보 거버넌스** 에서 **가져오기** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b747f-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="b747f-106">**가져오기 작업 유형 선택** 을 선택한 다음 **다음** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b747f-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="b747f-107">이 가져오기 옵션에 대한 단계를 보려면 **하드 드라이브를 실제 위치 중 하나로 배송** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="b747f-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="b747f-108">다음은 기억해야 할 몇 가지 사항입니다.</span><span class="sxs-lookup"><span data-stu-id="b747f-108">Here are some things to remember:</span></span>

- <span data-ttu-id="b747f-109">PST 파일을 Microsoft 365 사서함으로 가져오려면 Exchange Online에서 사서함 가져오기/내보내기 역할을 할당받아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b747f-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="b747f-110">20GB 보다 큰 PST의 경우 성능이 영향을받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b747f-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="b747f-111">2.5인치 SSD(반도체 드라이브) 또는 2.5인치/3.5인치 SATA II/III 내장 하드 드라이브만 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="b747f-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="b747f-112">PST 파일을 포함하는 하드 드라이브는 BitLocker로 암호화해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b747f-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="b747f-113">드라이브 발송을 사용하여 Microsoft 365 사서함에 PST 파일을 가져오는 데 드는 비용은 1GB의 데이터당 2,000원입니다.</span><span class="sxs-lookup"><span data-stu-id="b747f-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="b747f-114">드라이브 배송 방법을 사용하여 PST를 가져오는 방법에 대한 자세한 내용은 [드라이브 배송을 사용하여 조직의 PST 파일 가져오기](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b747f-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>