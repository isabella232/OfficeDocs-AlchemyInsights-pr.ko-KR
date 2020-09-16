---
title: 파일을 읽기 전용으로 열기
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745595"
---
# <a name="file-open-read-only"></a><span data-ttu-id="cdf04-102">파일을 읽기 전용으로 열기</span><span class="sxs-lookup"><span data-stu-id="cdf04-102">File open read-only</span></span>

<span data-ttu-id="cdf04-103">파일을 열 때 읽기 전용으로 열리는 것을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="cdf04-104">경우에 따라 인터넷에서 파일을 여는 경우와 같이 추가 보안을 위한 것이 고, 다른 시간에는 변경할 수 있는 설정 때문일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="cdf04-105">다음은 파일이 읽기 전용으로 열리는 몇 가지 시나리오와 해당 파일을 변경 하기 위해 수행할 수 있는 몇 가지 단계입니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="cdf04-106">**내 바이러스 백신으로 인해 읽기 전용으로 열기**</span><span class="sxs-lookup"><span data-stu-id="cdf04-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="cdf04-107">일부 바이러스 백신 프로그램은 보안상 안전 하지 않은 파일을 읽기 전용으로 여는 방법으로 보호할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="cdf04-108">이러한 설정을 조정 하는 방법에 대 한 자세한 내용은 바이러스 백신 공급자에 게 문의 해야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="cdf04-109">Bits Defender에는 응용 프로그램 제외 추가에 대 한 콘텐츠 (예: [Bitdefender Control Center에서 응용 프로그램 또는 프로세스 제외를 추가 하는 방법](https://aka.ms/AA6098i))가 포함 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="cdf04-110">**파일 속성이 읽기 전용으로 설정 되어 있습니까?**</span><span class="sxs-lookup"><span data-stu-id="cdf04-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="cdf04-111">파일을 마우스 오른쪽 단추로 클릭 하 고 속성을 선택 하 여 파일 속성을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="cdf04-112">읽기 전용 특성이 선택 되어 있으면 선택을 취소 하 고 확인을 클릭할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="cdf04-113">**콘텐츠가 제한 된 보기에 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="cdf04-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="cdf04-114">인터넷 및 기타 안전 하지 않은 위치의 파일에는 바이러스, 웜 또는 컴퓨터에 손상을 줄 수 있는 기타 유형의 맬웨어가 포함 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="cdf04-115">일반적으로 전자 메일 첨부 파일이 나 다운로드 한 파일을 포함 하는 경우도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="cdf04-116">컴퓨터를 보호 하기 위해 안전 하지 않을 수 있는 위치에 있는 파일은 제한 된 보기에서 열립니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="cdf04-117">제한 된 보기를 사용 하면 위험을 줄이면서 파일을 읽고 해당 내용을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="cdf04-118">제한 된 보기에 대 한 자세한 내용과 설정을 변경 하는 방법에 대 한 자세한 내용은 [제한 된 보기 란?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653) 문서를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="cdf04-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="cdf04-119">**OneDrive가 꽉 차서 있나요?**</span><span class="sxs-lookup"><span data-stu-id="cdf04-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="cdf04-120">파일이 OneDrive에 저장 되 고 OneDrive 저장소 공간이 가득 찬 경우 할당 된 공간에 도달할 때까지 문서를 저장할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="cdf04-121">알림 센터에서 OneDrive 아이콘을 클릭 하 고 저장소 관리를 선택 하 여 OneDrive의 사용 가능한 공간을 확인 하 고 [https://onedrive.live.com](https://onedrive.live.com) 화면 왼쪽 아래에 있는 사용 된 공간을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="cdf04-122">**Office 정품 인증 여부**</span><span class="sxs-lookup"><span data-stu-id="cdf04-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="cdf04-123">Office가 활성화 되지 않았거나 구독이 만료 된 경우에는 읽기 전용 기능 제한 모드로 설정 되어 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cdf04-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="cdf04-124">Office를 정품 인증 하는 방법에 대 한 자세한 내용은 [office의 사용 허가 되지 않은 제품 및 정품 인증 오류](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="cdf04-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="cdf04-125">**다른 모든 작업이 실패 하면 ...**</span><span class="sxs-lookup"><span data-stu-id="cdf04-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="cdf04-126">컴퓨터를 다시 시작 해 보십시오.</span><span class="sxs-lookup"><span data-stu-id="cdf04-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="cdf04-127">Office 업데이트 설치</span><span class="sxs-lookup"><span data-stu-id="cdf04-127">Install Office updates</span></span>
    
- <span data-ttu-id="cdf04-128">Office의 온라인 복구 수행</span><span class="sxs-lookup"><span data-stu-id="cdf04-128">Perform an Online repair of Office</span></span>
    

