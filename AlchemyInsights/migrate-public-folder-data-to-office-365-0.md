---
title: Microsoft 365로 공용 폴더 데이터 마이그레이션
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "639"
- "3500007"
ms.assetid: 6e536c7d-ab36-413e-9702-63e51adb3452
ms.openlocfilehash: 6dac268b3371af3a28bf8ef598e3a74d954a595c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707312"
---
# <a name="migrate-public-folder-data-to-microsoft-365"></a><span data-ttu-id="38f4a-102">Microsoft 365로 공용 폴더 데이터 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="38f4a-102">Migrate public folder data to Microsoft 365</span></span>

<span data-ttu-id="38f4a-103">Microsoft 365로 가져올 공용 폴더가 많지 않은 경우 데이터를 에 복사하는 가장 쉬운 방법은 에 데이터를 복사하는 것입니다. PST 파일을 가져온 다음 Microsoft 365로 가져와야 합니다.</span><span class="sxs-lookup"><span data-stu-id="38f4a-103">If you don't have a lot of public folders to bring into Microsoft 365, the easiest way to bring them would be to copy the data into .PST files and then import them into Microsoft 365.</span></span> <span data-ttu-id="38f4a-104">소량의 데이터의 경우 공용 폴더를 에 끌어서 놓기만 할 수 있습니다. PST 파일로 충분할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38f4a-104">For small amounts of data, a simple drag and drop of public folder into a .PST file can be sufficient.</span></span> <span data-ttu-id="38f4a-105">이보다 많은 데이터(최대 30GB)가 있는 [](https://technet.microsoft.com/library/dn874017%28v=exchg.150%29.aspx) 경우 폴더를 PST 파일로 내보내는 데 사용할 수 있는 프로세스를 문서화했습니다.</span><span class="sxs-lookup"><span data-stu-id="38f4a-105">If you have more data than that (up to 30GB), we have [documented a process](https://technet.microsoft.com/library/dn874017%28v=exchg.150%29.aspx) that you can use to export folders to PST files.</span></span>
  
<span data-ttu-id="38f4a-106">공용 폴더를 Microsoft 365로 이동하는 대규모 조직의 경우 다음 가이드를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38f4a-106">For larger organizations who are moving public folders into Microsoft 365, we have guides available:</span></span>
  
- <span data-ttu-id="38f4a-107">[레거시 공용 폴더 마이그레이션(Exchange](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/batch-migration-of-legacy-public-folders) 2010)</span><span class="sxs-lookup"><span data-stu-id="38f4a-107">[Migrate legacy public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/batch-migration-of-legacy-public-folders) (Exchange 2010)</span></span>

- [<span data-ttu-id="38f4a-108">Exchange 2013, Exchange 2016 또는 Exchange 2019 공용 폴더 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="38f4a-108">Migrate Exchange 2013, Exchange 2016, or Exchange 2019 public folders</span></span>](https://docs.microsoft.com/Exchange/collaboration/public-folders/migrate-to-exchange-online)

<span data-ttu-id="38f4a-109">공용 폴더를 [Microsoft 365 그룹으로 마이그레이션하는 옵션도 있습니다.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/migrate-your-public-folders-to-microsoft-365-groups)</span><span class="sxs-lookup"><span data-stu-id="38f4a-109">You also have the option to [migrate public folders to Microsoft 365 Groups](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/migrate-your-public-folders-to-microsoft-365-groups).</span></span>
  