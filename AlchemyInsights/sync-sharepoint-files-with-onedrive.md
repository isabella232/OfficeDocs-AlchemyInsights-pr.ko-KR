---
title: SharePoint Online의 "탐색기에서 열기" 문제 해결
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ba9f11da5c35c3681e9bd5ceaf13233fe8b80fc9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737311"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="4034f-102">SharePoint Online의 "탐색기에서 열기" 문제 해결</span><span class="sxs-lookup"><span data-stu-id="4034f-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="4034f-103">[요청 기반 파일 관리](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)를 제공하는[ 새 OneDrive 동기화 클라이언트와 SharePoint 파일을 동기화](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)하는 것이 좋습니다. 파일에 대한 로컬 액세스 권한과 최상의 성능을 제공하기 때문입니다.</span><span class="sxs-lookup"><span data-stu-id="4034f-103">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>

<span data-ttu-id="4034f-104">탐색기에서 열기 문제를 해결하려면 다음 문서에 나와있는 단계와 모범 사례를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="4034f-104">To troubleshoot Open with Explorer issues, follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="4034f-105">“탐색기에서 열기” 명령을 사용하여 SharePoint Online의 문제를 해결하는 방법</span><span class="sxs-lookup"><span data-stu-id="4034f-105">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)
- [<span data-ttu-id="4034f-106">탐색기에서 열기를 사용하여 라이브러리 파일 복사 또는 이동</span><span class="sxs-lookup"><span data-stu-id="4034f-106">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> <span data-ttu-id="4034f-107">**참고:**</span><span class="sxs-lookup"><span data-stu-id="4034f-107">**Note:**</span></span>
>- <span data-ttu-id="4034f-108">탐색기에서 열기는 Internet Explorer 10 또는 11에서만 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="4034f-108">Open with Explorer is only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="4034f-109">탐색기에서 열기는 Microsoft Edge가 포함된 Windows, Google Chrome, Mozilla Firefox, 또는 Mac 플랫폼에서 작동하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4034f-109">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="4034f-110">이러한 이유로, 탐색기 보기 옵션은 회색으로 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4034f-110">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
>- <span data-ttu-id="4034f-111">탐색기에서 열기 단추는 새 라이브러리 환경에 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4034f-111">The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="4034f-112">오른쪽 위의 **보기** 드롭다운(현재 보기에 따라 드롭다운 이름이 변경됨)을 클릭한 다음, **파일 탐색기에서 보기**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="4034f-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
