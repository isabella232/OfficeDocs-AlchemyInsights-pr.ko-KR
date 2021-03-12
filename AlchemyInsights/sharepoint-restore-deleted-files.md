---
title: 삭제된 파일 또는 폴더 복원
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
ms.openlocfilehash: 8c7ce48f50b5c933ea15c23a486b99ad7a7f4d79
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707528"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="9f179-102">삭제된 파일 또는 폴더 복원</span><span class="sxs-lookup"><span data-stu-id="9f179-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="9f179-103">SharePoint Online은 실제 삭제 후에도 14일 동안 모든 콘텐츠의 백업을 유지 합니다.</span><span class="sxs-lookup"><span data-stu-id="9f179-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="9f179-104">콘텐츠가 Recycle Bin 또는 Files Restore을 통해 복원될 수 없는 경우 관리자는 Microsoft 지원에 문의하여 14일 기간 안에 복원을 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9f179-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="9f179-105">백업에서의 복원은 특정 파일, 목록 또는 라이브러리가 아닌, 사이트 모음 또는 하위 사이트에 대해서만 가능합니다.</span><span class="sxs-lookup"><span data-stu-id="9f179-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="9f179-106">Sharepoint에서 항목 또는 사이트를 삭제하는 경우 즉시 제거되지는 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9f179-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="9f179-107">삭제된 항목은 일정 기간 동안 휴지통으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="9f179-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="9f179-108">해당 기간 동안 삭제한 항목을 원래 위치로 복원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9f179-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="9f179-109">자세한 내용을 보려면 아래 링크를 방문하세요.</span><span class="sxs-lookup"><span data-stu-id="9f179-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="9f179-110">[SharePoint 사이트의 Recycle Bin에](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be)있는 항목을 복원합니다.</span><span class="sxs-lookup"><span data-stu-id="9f179-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span></span>

[<span data-ttu-id="9f179-111">OneDrive에서 삭제된 파일 또는 폴더 복원</span><span class="sxs-lookup"><span data-stu-id="9f179-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="9f179-112">삭제된 사이트 모음 복원(그룹, 통신 및 기타 사이트 포함)</span><span class="sxs-lookup"><span data-stu-id="9f179-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="9f179-113">삭제된 OneDrive 사이트 복원</span><span class="sxs-lookup"><span data-stu-id="9f179-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="9f179-114">대량 재활용 쓰레기 수거통 작업의 경우 관리자는 [Sharepoint Online PNP를](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9f179-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="9f179-115">**파일 복원 기능**</span><span class="sxs-lookup"><span data-stu-id="9f179-115">**Files Restore feature**</span></span>

<span data-ttu-id="9f179-116">많은 OneDrive 또는 SharePoint 파일이 맬웨어에 의해 삭제, 덮어 사용, 손상 또는 감염되는 경우 파일 복원 기능을 사용하여 이전 시간으로 전체 OneDrive 또는 SharePoint 라이브러리를 복원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9f179-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="9f179-117">OneDrive 라이브러리 복원</span><span class="sxs-lookup"><span data-stu-id="9f179-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="9f179-118">문서 라이브러리 복원</span><span class="sxs-lookup"><span data-stu-id="9f179-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

