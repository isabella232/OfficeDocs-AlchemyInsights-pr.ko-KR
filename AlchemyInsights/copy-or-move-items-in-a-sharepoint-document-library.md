---
title: SharePoint 문서 라이브러리에서 항목 복사 또는 이동
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "454"
- "5300013"
ms.assetid: 592f502a-493f-4bf4-adc3-5bc8aea87bb5
ms.openlocfilehash: d7aa865a6b3db0871a57313dd7d6f5b0213ca0e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807125"
---
# <a name="copy-or-move-items-in-a-sharepoint-document-library"></a><span data-ttu-id="b80cd-102">SharePoint 문서 라이브러리에서 항목 복사 또는 이동</span><span class="sxs-lookup"><span data-stu-id="b80cd-102">Copy or move items in a SharePoint document library</span></span>

<span data-ttu-id="b80cd-103">문서 라이브러리 내에서 다른 위치로 파일, 폴더 및 링크를 복사 하 고 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b80cd-103">You can copy and move files, folders, and links to different locations within a document library.</span></span> <span data-ttu-id="b80cd-104">여러 사이트에서 항목을 복사할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b80cd-104">You can also copy items across sites.</span></span> 
  
1. <span data-ttu-id="b80cd-105">브라우저에서 이동할 파일, 폴더 또는 링크를 찾은 다음 **복사** **위치 또는로 이동을**클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="b80cd-105">In a browser, browse to the files, folders, or links you want to move, and then click **Copy to** or **Move to**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="b80cd-106">SharePoint Online의 클래식 환경을 사용 하는 경우에는 **복사 하기** 및 **이동을** 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b80cd-106">**Copy to** and **Move to** aren't available if you're using the classic experience of SharePoint Online.</span></span>
  
2. <span data-ttu-id="b80cd-107">**대상 선택**아래에서 항목을 복사 하거나 이동할 위치를 선택 하거나 사이트 **찾아보기를** 클릭 하 여 사이트의 전체 목록을 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="b80cd-107">Under **Choose a destination**, select the location to which you want to copy or move the items or click **Browse sites** to see the full list of sites.</span></span>

    > [!NOTE]
    > <span data-ttu-id="b80cd-108">항목을 복사할 때 다른 사이트가 표시 되지 않으면 사이트 간 복사가 구성 되지 않은 것입니다.</span><span class="sxs-lookup"><span data-stu-id="b80cd-108">If you don't see other sites listed when you copy items, copying across sites hasn't been configured.</span></span> <span data-ttu-id="b80cd-109">이 기능을 사용 하도록 설정 하려면 SharePoint 관리 센터의 설정 페이지로 이동한 후 **확인**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="b80cd-109">To enable it, go to the settings page of the SharePoint admin center and click **OK**.</span></span>
  
    <span data-ttu-id="b80cd-110">새 폴더를 만들려면 폴더 계층 구조에서 위치를 선택 하 고 **새 폴더**를 클릭 하 고 폴더 이름을 입력 한 다음 확인 표시를 클릭 하 여 이름을 저장 합니다.</span><span class="sxs-lookup"><span data-stu-id="b80cd-110">To create a new folder, select a location in the folder hierarchy, click **New folder**, enter a name for the folder, and click the check mark to save the name.</span></span>

3. <span data-ttu-id="b80cd-111">**여기로 복사** 또는 **여기로 이동을**클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="b80cd-111">Click **Copy here** or **Move here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="b80cd-112">한 번에 최대 500 MB의 파일 및 폴더를 복사할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b80cd-112">You can copy up to 500 MB of files and folders at one time.</span></span> <span data-ttu-id="b80cd-113">> 버전 기록이 포함 된 문서를 복사할 때 최신 버전만 복사 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b80cd-113">>  When you copy documents that have version history, only the latest version is copied.</span></span> <span data-ttu-id="b80cd-114">문서를 이동 하면 해당 기록도 이동 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b80cd-114">When you move documents, their history is also moved.</span></span>
  
 <span data-ttu-id="b80cd-115">파일을 이동 하는 경우 해당 파일이 대상으로 완전히 이동 될 때까지 원본 디렉터리에 계속 표시 되 고 삭제 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b80cd-115">When a file is moving, it will still appear in the source directory until its fully moved to the destination, and then it will be deleted.</span></span> <span data-ttu-id="b80cd-116">파일은 이동이 완료 된 후 원본 사이트 휴지통에 유지 되 고 사용자가 휴지통에서 복구 하는 경우를 제외 하 고 일반 재활용 일정이 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b80cd-116">The file will remain in the source sites recycle bin after the move is complete and be subject to the normal recycle schedule unless a user recovers it from the recycle bin.</span></span>

<span data-ttu-id="b80cd-117">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b80cd-117">For more information, see:</span></span>

 - <span data-ttu-id="b80cd-118">[SharePoint에서 파일 이동 또는 복사](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office 지원 문서)</span><span class="sxs-lookup"><span data-stu-id="b80cd-118">[Move or copy files in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office support article)</span></span>
 - <span data-ttu-id="b80cd-119">[모든 폴더에서 파일 이동](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft 기술 커뮤니티 블로그 문서)</span><span class="sxs-lookup"><span data-stu-id="b80cd-119">[Move files from any folder](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span></span>  