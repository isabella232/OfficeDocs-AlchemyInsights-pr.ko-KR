---
title: nk2-파일을 가져오는 방법
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780065"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="a38d4-102">Nk2 파일을 가져오는 방법</span><span class="sxs-lookup"><span data-stu-id="a38d4-102">How to import .nk2 files</span></span> 

<span data-ttu-id="a38d4-103">Microsoft Outlook 2013, Outlook 2016, Outlook 2019 또는 Outlook for Microsoft 365을 처음 시작 하면 *profilename*파일에 저장 된 애칭 캐시를 기본 메시지 저장소의 숨겨진 메시지로 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="a38d4-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="a38d4-104">Nk2 파일을 Outlook 2013, Outlook 2016, Outlook 2019 또는 Microsoft 365 Outlook으로 가져오려면 nk2 파일이 다음 폴더에 있는지 확인 하십시오 .%appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="a38d4-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="a38d4-105">**참고**: nk2 파일의 이름은 현재 outlook 2013 또는 Outlook 2016 프로필과 이름이 같아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a38d4-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="a38d4-106">기본적으로 프로필 이름은 "Outlook"입니다.</span><span class="sxs-lookup"><span data-stu-id="a38d4-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="a38d4-107">프로필 이름을 확인 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="a38d4-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="a38d4-108">**시작**을 클릭하고 **제어판**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="a38d4-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="a38d4-109">**메일**을 두 번 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a38d4-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="a38d4-110">메일 설정 대화 상자에서 **프로필 보기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="a38d4-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="a38d4-111">실행 **시작**  >  **Run**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="a38d4-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="a38d4-112">**열기** 상자에 *outlook.exe/importnk2*를 입력 하 고 **확인**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="a38d4-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="a38d4-113">Nk2 파일을 가져온 후에는 파일의 내용이 사서함에 저장 된 기존 애칭 캐시에 병합 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a38d4-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="a38d4-114">**참고**: nk2 파일의 이름은 다음에 outlook 2013, outlook 2016, outlook 2019 또는 Microsoft 365 outlook을 시작할 때 .old 파일 이름 확장명으로 바뀝니다.</span><span class="sxs-lookup"><span data-stu-id="a38d4-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365.</span></span> <span data-ttu-id="a38d4-115">Nk2 파일을 다시 가져오려면 먼저 .old 파일 이름 확장명을 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="a38d4-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="a38d4-116">자세한 내용은 [자동 완성 목록을 다른 컴퓨터에 가져오기 또는 복사](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="a38d4-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>