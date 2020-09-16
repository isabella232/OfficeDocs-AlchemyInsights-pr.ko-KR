---
title: SharePoint 또는 OneDrive에서 액세스 제한
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720688"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="77c87-102">SharePoint 또는 OneDrive에서 액세스 제한</span><span class="sxs-lookup"><span data-stu-id="77c87-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="77c87-103">SharePoint 및 OneDrive에서는 액세스할 그룹 또는 개인 에게만 액세스 권한을 부여 하 여 파일, 폴더 및 목록 등의 항목에 대 한 액세스를 제한 합니다.</span><span class="sxs-lookup"><span data-stu-id="77c87-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="77c87-104">기본적으로 SharePoint의 사용 권한은 계층 구조에서 위쪽 으로부터 상속 됩니다.</span><span class="sxs-lookup"><span data-stu-id="77c87-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="77c87-105">따라서 파일은 해당 폴더의 사용 권한을 상속 하며, 사이트에서 사용 권한을 상속 하는 라이브러리의 사용 권한을 상속 합니다.</span><span class="sxs-lookup"><span data-stu-id="77c87-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="77c87-106">사이트의 모든 항목을 공유 하지 않으려면 더 높은 수준 (예: 전체 사이트를 공유 함)으로 공유한 다음 상속을 끊는 것을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="77c87-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="77c87-107">그러나 이후에는 사용 권한을 보다 복잡 하 고 혼동 하기 때문에이 방법을 사용 하지 않는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="77c87-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="77c87-108">이 작업을 대신 수행할 수 있는 작업은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="77c87-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="77c87-109">예를 들어 파일 하나를 제외 하 고 폴더의 모든 내용을 공유 하려면 해당 파일을 공유 하지 않는 새 위치로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="77c87-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="77c87-110">폴더에 하위 폴더가 두 개 있는 경우 하나의 하위 폴더를 그룹 A 및 B와 공유 하 고 두 번째 하위 폴더에 대 한 액세스만 허용 하려면 상위 폴더를 그룹 A와 공유 하 고 그룹 B를 첫 번째 하위 폴더에 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="77c87-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="77c87-111">파일 또는 폴더 공유 중지 </span><span class="sxs-lookup"><span data-stu-id="77c87-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

