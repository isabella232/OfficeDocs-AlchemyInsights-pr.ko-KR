---
title: SharePoint Designer 연결 문제
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
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727177"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="56d7b-102">SharePoint Designer 연결 문제</span><span class="sxs-lookup"><span data-stu-id="56d7b-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="56d7b-103">SharePoint Designer에 SharePoint 사이트에 대 한 연결 문제가 발생 하는 경우 다음과 같은 일반적인 해결 방법을 시도해 보세요.</span><span class="sxs-lookup"><span data-stu-id="56d7b-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="56d7b-104">1 단계: sharepoint designer 2013이 sharepoint designer [서비스 팩 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) 과 [8 월 2 일, 2016 Update for sharepoint designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)에 업데이트 되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="56d7b-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="56d7b-105">2 단계: 로컬 캐시 파일 지우기:</span><span class="sxs-lookup"><span data-stu-id="56d7b-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="56d7b-106">SharePoint Designer 2013을 닫습니다.</span><span class="sxs-lookup"><span data-stu-id="56d7b-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="56d7b-107">로컬 컴퓨터에서 다음 폴더 각각에 있는 파일을 모두 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="56d7b-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="56d7b-108">%APPDATA%\Microsoft\Web 서버 Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="56d7b-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="56d7b-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="56d7b-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="56d7b-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="56d7b-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="56d7b-111">SharePoint Designer 2013를 열고 계정을 다시 입력 하 여 작동 하는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="56d7b-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="56d7b-112">3 단계: [Windows 장치에서 Office 2013에 대 한 최신 인증을 사용 하도록 설정](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)합니다.</span><span class="sxs-lookup"><span data-stu-id="56d7b-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="56d7b-113">4 단계: 관리자는 sharepoint 관리 센터 설정에서 **사용자 지정 스크립트를 허용** 하 여이 연결을 허용 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="56d7b-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="56d7b-114">자세한 내용은 [사용자 지정 스크립트 허용 또는 금지](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="56d7b-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


