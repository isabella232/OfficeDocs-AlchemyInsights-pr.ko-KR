---
title: Yammer에서 이미지 로딩 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146803"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="a1443-102">Yammer에서 이미지 로딩 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a1443-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="a1443-103">Yammer에서 사진 및 파일 미리 보기와 관련 된 문제가 발생하면 모든 사용자에게 해당 문제가 발생하는지 여부를 확인하고, 모바일 장치에서 발생하는지, 첨부 파일을 업로드할 때 복사 할 수 있는지 확인하여 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="a1443-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="a1443-104">**프로필 사진 문제**</span><span class="sxs-lookup"><span data-stu-id="a1443-104">**Profile photo issues**</span></span>  

<span data-ttu-id="a1443-105">최종 사용자가 Microsoft 365를 통해 Yammer에 로그인하는 경우 프로필 사진을 포함하여 프로필을 변경해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a1443-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="a1443-106">사용자가 프로필 업데이트를 수행할 수 없는 경우 관리자가 사용자를 위해 업데이트 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a1443-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="a1443-107">자세한 내용은 [Office Delve에서 프로필 보기 및 업데이트](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a1443-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="a1443-108">프로필 사진을 포함하여 프로필 편집에 대한 자세한 내용은 [Yammer 프로필과 설정 변경](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a1443-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="a1443-109">업데이트 된 프로필 사진은 프로필 속성과 다르게 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a1443-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="a1443-110">사용자가 프로필 사진의 동기화를 시작 하려면 로그인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a1443-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="a1443-111">자세한 내용은 [사용자 프로필 사진이 Office 365에서 Yammer로 업데이트 되나요](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a1443-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="a1443-112">Yammer의 사용자 수명 주기에 대한 자세한 내용은 [Office 365에서 수명 주기 동안 Yammer 사용자 관리](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a1443-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="a1443-113">Microsoft 365에서 프로필 사진 동기화가 적용 되는 방법에 대한 자세한 내용은 [Microsoft 365에서 프로필 사진 동기화 정보](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="a1443-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="a1443-114">**문서 미리 보기 및 이미지 축소판 그림 문제**</span><span class="sxs-lookup"><span data-stu-id="a1443-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="a1443-115">파일이나 이미지를 Yammer에 게시 할 때 다음 때문에 미리 보기가 표시 되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a1443-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="a1443-116">파일이 손상되어 처리할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="a1443-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="a1443-117">최근에 SharePoint Online에 파일이 업로드 되지 않은 경우 또는 Yammer에 다른 이유로 인해 잘못 된 메타 데이터가 있는 경우</span><span class="sxs-lookup"><span data-stu-id="a1443-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="a1443-118">미리보기 이미지를 로딩하는데 필요한 URL은 차단됩니다.</span><span class="sxs-lookup"><span data-stu-id="a1443-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="a1443-119">파일 미리보기는 게시 전에 사용자에 의해 제거 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a1443-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="a1443-120">서비스 문제 때문에 미리 보기를 생성할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="a1443-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="a1443-121">**알림** 링크와 파일 업로드 미리보기가 다르게 작동 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a1443-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="a1443-122">추가 인증이 필요한 인터넷 혹은 링크에서 파일 링크가 올바르게 표시되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a1443-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="a1443-123">자세한 내용은 [Yammer 메시지에 파일 또는 이미지 첨부](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a1443-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 