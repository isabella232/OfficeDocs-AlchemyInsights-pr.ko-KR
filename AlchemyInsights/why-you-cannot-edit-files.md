---
title: 파일 편집을 위해 잠김
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "9000123"
- "1622"
- "1713"
ms.openlocfilehash: 3020837e8e8dd3b9ff4ada33f23c6118e83c3806
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664500"
---
# <a name="why-cant-i-edit-files"></a><span data-ttu-id="6df2d-102">파일을 편집할 수 없는 이유는 무엇 인가요?</span><span class="sxs-lookup"><span data-stu-id="6df2d-102">Why can't I edit files?</span></span>

<span data-ttu-id="6df2d-103">[파일을 편집 하지 못할 수](https://support.office.com/article/why-can-t-i-edit-this-file-97315f48-aa5e-49d3-a4ae-a14b73daf87b)있는 몇 가지 이유를 간략하게 살펴봅니다.</span><span class="sxs-lookup"><span data-stu-id="6df2d-103">Take a quick look at some of the reasons [why you might not be able to edit the file](https://support.office.com/article/why-can-t-i-edit-this-file-97315f48-aa5e-49d3-a4ae-a14b73daf87b).</span></span>

<span data-ttu-id="6df2d-104">**체크 아웃, 필수** 또는 **유효성 검사** 열 또는 메타 데이터를 포함 하는 라이브러리가 있거나 라이브러리의 버전 설정에서 **항목을 승인할 수** 있는 사용자 **만** 이 **초안 항목 보안** 을 설정 하는 경우:</span><span class="sxs-lookup"><span data-stu-id="6df2d-104">If you have libraries with **Checkout, Required** or **Validation** columns or metadata, or when **Draft Item Security** is set to either **Only users who can edit** or **Only users who can approve items** in Version Settings of the library:</span></span>

- <span data-ttu-id="6df2d-105">SharePoint 문서 라이브러리의 경우 이러한 항목은 읽기 전용으로 동기화 됩니다.</span><span class="sxs-lookup"><span data-stu-id="6df2d-105">For SharePoint document libraries, these items will be synchronized as read-only.</span></span>

- <span data-ttu-id="6df2d-106">OneDrive 라이브러리의 경우 OneDrive에서 동기화 상태 옆에 잠금 아이콘 (OneDrive 파일 잠김 아이콘)이 표시 되 고, 앞에서 설명한 설정이 제거 될 때까지 사용자가 라이브러리를 동기화 할 수 없게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="6df2d-106">For OneDrive libraries, OneDrive will show a lock icon ( OneDrive file locked icon ) next to the sync status and the user will not be able to synchronize the library until the mentioned settings have been removed.</span></span> 

<span data-ttu-id="6df2d-107">Word 또는 Excel의 잠긴 파일에 대 한 자세한 내용은 아래 문서를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="6df2d-107">For more information regarding locked files for Word or Excel, please reference the articles below.</span></span>

- [<span data-ttu-id="6df2d-108">Office 파일을 편집 하는 동안 "업로드 하지 못했습니다." 또는 "자동으로 저장할 수 없습니다." 오류가 발생 함</span><span class="sxs-lookup"><span data-stu-id="6df2d-108">I got an "Upload failed" or "Couldn't save automatically" error while editing an Office file</span></span>](https://support.office.com/article/i-got-an-upload-failed-or-couldn-t-save-automatically-error-while-editing-an-office-file-93a14d34-88e3-4a91-9eef-58cc541d31f8)

- [<span data-ttu-id="6df2d-109">다른 사용자가 Excel 파일을 편집용으로 잠 궜 습니다.</span><span class="sxs-lookup"><span data-stu-id="6df2d-109">Excel file is locked for editing by another user</span></span>](https://support.office.com/article/Excel-file-is-locked-for-editing-by-another-user-6fa93887-2c2c-45f0-abcc-31b04aed68b3)

- [<span data-ttu-id="6df2d-110">다른 사용자가 Word 파일을 편집용으로 잠 궜 습니다.</span><span class="sxs-lookup"><span data-stu-id="6df2d-110">Word file is locked for editing by another user</span></span>](https://support.microsoft.com/help/313472/the-document-is-locked-for-editing-by-another-user-error-message-when)
