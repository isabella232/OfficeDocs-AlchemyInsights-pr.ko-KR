---
title: Bing에서 Microsoft Search의 배경 서비스 제거
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753443"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="8e85d-102">Bing에서 Microsoft Search의 배경 서비스 제거</span><span class="sxs-lookup"><span data-stu-id="8e85d-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="8e85d-103">Bing에서 Microsoft Search의 배경 서비스를 제거하려면 다음 방법을 시도해 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8e85d-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="8e85d-104">원래 검색 엔진 설정으로 되돌리려면 다음 작업을 수행하세요.</span><span class="sxs-lookup"><span data-stu-id="8e85d-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="8e85d-105">a.</span><span class="sxs-lookup"><span data-stu-id="8e85d-105">a.</span></span> <span data-ttu-id="8e85d-106">**Bing을 기본 검색 엔진으로 사용[ 토글을](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)끄기** 로 전환합니다.</span><span class="sxs-lookup"><span data-stu-id="8e85d-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="8e85d-107">b.</span><span class="sxs-lookup"><span data-stu-id="8e85d-107">b.</span></span> <span data-ttu-id="8e85d-108">[Microsoft 365 관리 센터로 이동](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed)하여조직의 모든 사용자에게 영향을 주는 설정을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="8e85d-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="8e85d-109">개별 장치에서 배경 서비스를 제거하려면 다음 작업을 수행하세요.</span><span class="sxs-lookup"><span data-stu-id="8e85d-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="8e85d-110">a.</span><span class="sxs-lookup"><span data-stu-id="8e85d-110">a.</span></span> <span data-ttu-id="8e85d-111">**제어판 > 프로그램 > 프로그램 및 기능** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8e85d-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="8e85d-112">b.</span><span class="sxs-lookup"><span data-stu-id="8e85d-112">b.</span></span> <span data-ttu-id="8e85d-113">설치된 프로그램 목록에서 **Bing의 Microsoft Search** 를 마우스 오른쪽 단추로 클릭한 다음 **제거** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="8e85d-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="8e85d-114">조직의 여러 장치에서 배경 서비스를 제거하려면 관리자로 로그인하고 스크립트에서 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="8e85d-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
