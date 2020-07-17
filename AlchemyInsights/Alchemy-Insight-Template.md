---
title: 파일 이름과 동일
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750976"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="67cc1-102">"필수 Alchemy 헤더 H1, H2's이 작동 하지 않음"</span><span class="sxs-lookup"><span data-stu-id="67cc1-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="67cc1-103">Alchemy 작성을 위한 모범 사례 및 지침:</span><span class="sxs-lookup"><span data-stu-id="67cc1-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="67cc1-104">**Alchemy Insights를 폴더에 중첩 하지 마세요**-url 구조가 손상 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67cc1-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="67cc1-105">여기서는이 문제를 해결 하 고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67cc1-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="67cc1-106">**AlchemyInsights** 폴더의 파일에는 공백 하이픈을 포함 하는 소문자 파일 이름이 포함 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67cc1-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="67cc1-107">***사용 방법-설정-소송-보존***</span><span class="sxs-lookup"><span data-stu-id="67cc1-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="67cc1-108">[Alchemy 파트너 포털](https://alchemyportal.azurewebsites.net) 의 사용자 정의 필드에 규칙 ID 또는 버킷 id를 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="67cc1-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="67cc1-109">ex.</span><span class="sxs-lookup"><span data-stu-id="67cc1-109">ex.</span></span> <span data-ttu-id="67cc1-110">***사용자 지정: 100021***</span><span class="sxs-lookup"><span data-stu-id="67cc1-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="67cc1-111">이 파일의 맨 위에 있는 메타 데이터의 나머지 부분을 서식 파일로 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="67cc1-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="67cc1-112">[Alchemy 파트너 포털](https://alchemyportal.azurewebsites.net)에서 **고객 통찰력 제목** 섹션으로 이동한 다음 해당 내용을 H1 제목에 대 한 시작 점으로 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="67cc1-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="67cc1-113">Alchemy Insights는 맨 위에 단일 H1만 포함 되거나 프로덕션에서 중단 됩니다.</span><span class="sxs-lookup"><span data-stu-id="67cc1-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="67cc1-114">H2s은 렌더링 되지 않으므로 별도의 섹션을 나타내기 위해 **굵게** 또는 기타 규칙을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="67cc1-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="67cc1-115">다음으로, Alchemy 규칙 페이지의 Customer Insights 섹션에 있는 초안 자료를 사용 하 여 본문 텍스트를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="67cc1-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="67cc1-116">글머리 기호 목록이 양호 함</span><span class="sxs-lookup"><span data-stu-id="67cc1-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="67cc1-117">번호 매기기 목록만 너무 많이 있음</span><span class="sxs-lookup"><span data-stu-id="67cc1-117">Numbered lists too</span></span>
    1. <span data-ttu-id="67cc1-118">**굵게** 및 *기울임꼴로* 표시 되는-정상</span><span class="sxs-lookup"><span data-stu-id="67cc1-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="67cc1-119">링크는 항상 내부 링크가 아니라 **UI 요소에 대**한 **"웹 연결"/외부** 또는 딥 링크 중 하나 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="67cc1-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="67cc1-120">이때 그림은 공식적으로 지원 되는 것은 아니지만 로드맵에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="67cc1-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="67cc1-121">이는 실제로 너무 긴 시간입니다.</span><span class="sxs-lookup"><span data-stu-id="67cc1-121">And this is really already a bit too long.</span></span> <span data-ttu-id="67cc1-122">모범 사례는 약 400 자---------------------------------</span><span class="sxs-lookup"><span data-stu-id="67cc1-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="67cc1-123">콘텐츠가 준비 되 면 라이브 분기로 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="67cc1-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="67cc1-124">그런 다음 [Alchemy 파트너 포털로](https://alchemyportal.azurewebsites.net) 이동 하 여 url 필드에 파일 이름을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="67cc1-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 