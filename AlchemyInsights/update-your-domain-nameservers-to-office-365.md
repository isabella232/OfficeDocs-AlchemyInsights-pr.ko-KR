---
title: Microsoft를 가리키도록 도메인 이름 서버 업데이트
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 9dd52c60b2d15d66c1c3f2a96c9db08ea2a010c6
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510290"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="5713c-102">Microsoft를 가리키도록 도메인 이름 서버 업데이트</span><span class="sxs-lookup"><span data-stu-id="5713c-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="5713c-103">참고: 네임 서버 변경 사항이 전파되는 데 최대 48 시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5713c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="5713c-104">Microsoft에서 도메인을 설정 하려면 등록자에서 이름 서버를 업데이트 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5713c-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="5713c-105">도메인 등록 기관에서 이름 서버 레코드를 만들거나 편집합니다.</span><span class="sxs-lookup"><span data-stu-id="5713c-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="5713c-106">도메인 등록 기관 웹 사이트에서 이름 서버를 편집하는 곳을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="5713c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="5713c-107">아래의 값을 갖는 2개의 이름 서버 레코드를 만들거나 편집합니다.</span><span class="sxs-lookup"><span data-stu-id="5713c-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="5713c-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="5713c-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="5713c-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="5713c-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="5713c-110">변경 내용을 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="5713c-110">Save changes.</span></span>

<span data-ttu-id="5713c-111">또한이 문서에서 [이름 서버를 변경 하 여 도메인 등록 기관으로 Microsoft 365을 설정 하](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar) 는 방법에 대 한 자세한 지침을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5713c-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  