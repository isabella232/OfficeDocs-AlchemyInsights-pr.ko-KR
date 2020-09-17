---
title: 삭제 된 파일 또는 폴더 복원
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: fc560686ec5c6a3d42a97687fda80ae5001b5c60
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797554"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="92d04-102">삭제 된 파일 또는 폴더 복원</span><span class="sxs-lookup"><span data-stu-id="92d04-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="92d04-103">SharePoint Online은 실제 삭제 후에도 14일 동안 모든 콘텐츠의 백업을 유지 합니다.</span><span class="sxs-lookup"><span data-stu-id="92d04-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="92d04-104">휴지통 또는 파일 복원을 통해 콘텐츠를 복원할 수 없는 경우 관리자는 Microsoft 지원에 문의 하 여 14 일 내에 언제 든 지 복원을 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="92d04-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="92d04-105">백업에서의 복원은 특정 파일, 목록 또는 라이브러리가 아닌, 사이트 모음 또는 하위 사이트에 대해서만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="92d04-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="92d04-106">Sharepoint에서 항목 또는 사이트를 삭제 하면 즉시 제거 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="92d04-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="92d04-107">삭제된 항목은 일정 기간 동안 휴지통으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="92d04-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="92d04-108">해당 기간 동안 삭제한 항목을 원래 위치로 복원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="92d04-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="92d04-109">자세한 내용을 보려면 아래 링크를 방문하세요.</span><span class="sxs-lookup"><span data-stu-id="92d04-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="92d04-110">[SharePoint 사이트의 휴지통에 있는 항목을 복원](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b)합니다.</span><span class="sxs-lookup"><span data-stu-id="92d04-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="92d04-111">OneDrive에서 삭제 된 파일 또는 폴더 복원</span><span class="sxs-lookup"><span data-stu-id="92d04-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="92d04-112">삭제 된 사이트 모음 복원 (그룹, 통신 및 기타 사이트 포함)</span><span class="sxs-lookup"><span data-stu-id="92d04-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="92d04-113">삭제 된 OneDrive 사이트 복원</span><span class="sxs-lookup"><span data-stu-id="92d04-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="92d04-114">대량 휴지통 작업의 경우 관리자는 [Sharepoint ONLINE PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)를 사용 하는 것으로 간주 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="92d04-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="92d04-115">**파일 복원 기능**</span><span class="sxs-lookup"><span data-stu-id="92d04-115">**Files Restore feature**</span></span>

<span data-ttu-id="92d04-116">OneDrive 또는 SharePoint 파일의 수가 너무 많이 삭제, 덮어쓰기, 손상 또는 감염 된 경우 파일 복원 기능을 사용 하 여 전체 OneDrive 또는 SharePoint 라이브러리를 이전 시간으로 복원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="92d04-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="92d04-117">OneDrive 라이브러리 복원</span><span class="sxs-lookup"><span data-stu-id="92d04-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="92d04-118">문서 라이브러리 복원</span><span class="sxs-lookup"><span data-stu-id="92d04-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

