---
title: Verify your domain
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
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770997"
---
# <a name="verify-your-domain"></a><span data-ttu-id="491a0-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="491a0-102">Verify your domain</span></span>

 <span data-ttu-id="491a0-103">**레코드가 인터넷을 통해 업데이트되지 않은 것일 수 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="491a0-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="491a0-104">일반적으로 Microsoft에서 새 레코드를 확인하는 데 몇 분 정도면 되지만 경우에 따라 몇 시간이 걸릴 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="491a0-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="491a0-105">오래 기다렸다가 이미 기다렸다면 정확한 값을 복사하여 DNS 호스트의 TXT 확인 레코드에 붙여넣은 것이지 다시 한 번 확인하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="491a0-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="491a0-106">한 가지 일반적인 문제는 레코드의 "MS =" 부분을 포함하지 않는 경우입니다.</span><span class="sxs-lookup"><span data-stu-id="491a0-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="491a0-107">누락하지 않도록 주의하세요!</span><span class="sxs-lookup"><span data-stu-id="491a0-107">We need that too!</span></span>

- <span data-ttu-id="491a0-108">일부 DNS 호스트에서는 영역 파일(DNS 레코드가 저장되는 위치)이 인터넷을 통해 업데이트되도록 저장하는 추가 단계를 진행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="491a0-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="491a0-109">Microsoft에서 레코드를 보고 확인할 수 있도록 변경 내용을 저장해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="491a0-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
