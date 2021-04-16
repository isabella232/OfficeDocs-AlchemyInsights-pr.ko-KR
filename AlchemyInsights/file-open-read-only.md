---
title: 파일 열기 읽기 전용
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813190"
---
# <a name="file-open-read-only"></a><span data-ttu-id="fb143-102">파일 열기 읽기 전용</span><span class="sxs-lookup"><span data-stu-id="fb143-102">File open read-only</span></span>

<span data-ttu-id="fb143-103">파일을 열 때 읽기 전용으로 열립니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="fb143-104">경우에 따라 인터넷에서 파일을 여는 경우와 같은 추가 보안을 위한 것이고, 다른 경우에는 변경할 수 있는 설정 때문일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="fb143-105">다음은 파일이 읽기 전용으로 열리며 이를 변경하기 위해 취할 수 있는 몇 가지 단계입니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="fb143-106">**바이러스 백신으로 인해 읽기 전용이 열립니다.**</span><span class="sxs-lookup"><span data-stu-id="fb143-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="fb143-107">일부 바이러스 백신 프로그램은 읽기 전용으로 열면 안전하지 않을 수 있는 파일로부터 보호할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="fb143-108">이러한 설정을 조정하는 방법을 알아보기 위해 바이러스 백신 공급자에 문의해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="fb143-109">예를 들어 BitDefender에는 [Bitdefender](https://aka.ms/AA6098i)제어 센터에서 응용 프로그램 또는 프로세스 제외를 추가하는 방법에서 응용 프로그램 제외를 추가하는 방법에 대한 콘텐츠가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="fb143-110">**파일 속성이 읽기 전용으로 설정되어 있나요?**</span><span class="sxs-lookup"><span data-stu-id="fb143-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="fb143-111">파일을 마우스 오른쪽 단추로 클릭하고 속성을 선택하여 파일 속성을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="fb143-112">읽기 전용 특성이 선택된 경우 선택을 언하고 확인을 클릭할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="fb143-113">**콘텐츠가 보호된 보기에 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="fb143-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="fb143-114">인터넷 및 안전하지 않은 다른 위치의 파일에는 컴퓨터를 손상할 수 있는 바이러스, 웜 또는 기타 종류의 맬웨어가 포함될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="fb143-115">이는 일반적으로 다운로드한 전자 메일 첨부 파일이나 파일에서도 해당됩니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="fb143-116">컴퓨터를 보호하기 위해 안전하지 않은 위치의 파일이 보호된 보기에서 열립니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="fb143-117">보호된 보기를 사용하면 파일을 읽고 해당 내용을 볼 수 있으며 위험을 줄일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="fb143-118">보호된 보기 및 설정을 변경하는 방법에 대한 자세한 내용은 이 문서를 [참조하세요. 보호된 보기란?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="fb143-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="fb143-119">**OneDrive가 가득 있습니까?**</span><span class="sxs-lookup"><span data-stu-id="fb143-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="fb143-120">파일이 OneDrive에 저장되어 있으며 OneDrive 저장소 공간이 가득 차면 사용자가 사용 공간 아래에 있을 때까지 문서를 저장할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="fb143-121">알림 센터에서 OneDrive 아이콘을 클릭하고 저장소 관리를 선택하여 OneDrive에서 사용 공간을 확인하거나, 로 이동하여 화면 왼쪽 아래에서 사용된 공간의 양을 확인할 수 [https://onedrive.live.com](https://onedrive.live.com) 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="fb143-122">**Office가 정품 인증되어 있나요?**</span><span class="sxs-lookup"><span data-stu-id="fb143-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="fb143-123">Office가 정품 인증되지 않은 경우 또는 구독이 만료된 경우 읽기 전용 기능 제한 모드에 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fb143-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="fb143-124">Office 정품 인증 방법에 대한 자세한 내용은 Office의 라이선스가 없는 제품 및 정품 인증 [오류를 참조하세요.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="fb143-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="fb143-125">**다른 모든 오류가 발생하면...**</span><span class="sxs-lookup"><span data-stu-id="fb143-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="fb143-126">컴퓨터 다시 시작 시도</span><span class="sxs-lookup"><span data-stu-id="fb143-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="fb143-127">Office 업데이트 설치</span><span class="sxs-lookup"><span data-stu-id="fb143-127">Install Office updates</span></span>
    
- <span data-ttu-id="fb143-128">Office의 온라인 복구 수행</span><span class="sxs-lookup"><span data-stu-id="fb143-128">Perform an Online repair of Office</span></span>
    

