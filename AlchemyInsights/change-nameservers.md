---
title: 이름 서버 변경
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818618"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="709d1-102">Microsoft를 가리키도록 도메인 이름 서버 업데이트</span><span class="sxs-lookup"><span data-stu-id="709d1-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="709d1-103">참고: 네임 서버 변경 사항이 전파되는 데 최대 48 시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="709d1-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="709d1-p101">Microsoft 365에서 도메인을 설정하려면 등록 기관의 이름 서버를 업데이트해야 합니다. 도메인 등록 기관에서 이름 서버 레코드를 만들거나 편집합니다.</span><span class="sxs-lookup"><span data-stu-id="709d1-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="709d1-106">도메인 등록 기관 웹 사이트에서 이름 서버를 편집하는 곳을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="709d1-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="709d1-107">아래의 값을 갖는 2개의 이름 서버 레코드를 만들거나 편집합니다.</span><span class="sxs-lookup"><span data-stu-id="709d1-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="709d1-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="709d1-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="709d1-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="709d1-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="709d1-110">변경 내용을 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="709d1-110">Save changes.</span></span>

<span data-ttu-id="709d1-111">다음 문서에서도 자세한 방법을 확인할 수 있습니다. [도메인 등록 기관에서 이름 서버 변경](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="709d1-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  