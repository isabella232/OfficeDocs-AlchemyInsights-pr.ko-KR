---
title: 125 웹용 Outlook에서 잘못 된 라이선스 오류를 가져옵니다.
ms.author: daeite
author: daeite
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "125"
- "1600021"
ms.assetid: 6d9947d9-6c92-4ada-b655-8ab2a0c2b66d
ms.openlocfilehash: 825d91cd81646767b100e6fc964d7a94b8bc6879
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677465"
---
# <a name="getting-an-invalid-license-error-in-outlook-on-the-web"></a><span data-ttu-id="1db66-102">웹용 Outlook에서 잘못 된 라이선스 오류가 발생 하는 경우</span><span class="sxs-lookup"><span data-stu-id="1db66-102">Getting an invalid license error in Outlook on the web?</span></span>

<span data-ttu-id="1db66-103">웹에서 Outlook을 사용 하는 경우에는 **InvalidLicenseException**, exchange Online 라이선스가 올바르게 할당 되지 않았거나 최근에 만료 되지 않은 **것으로 나타나는 오류가 발생** 하는 것을 알 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1db66-103">If you're using Outlook on the web and you get a **Something went wrong** error that contains **X-OWA-Error: Microsoft.Exchange.Data.Storage.InvalidLicenseException**, your Exchange Online license isn't correctly assigned or has recently expired.</span></span> <span data-ttu-id="1db66-104">관리자는 다음 단계를 수행 하 여 라이선스를 사용자에 게 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1db66-104">Your admin can assign a license to you by following these steps:</span></span>
  
1. <span data-ttu-id="1db66-105">[Microsoft 365 관리 센터](https://portal.office.com/adminportal/home#/homepage) 를 열고 **활성 사용자**에서 **사용자 편집**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1db66-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and under **Active users**, select **Edit a user**.</span></span>

2. <span data-ttu-id="1db66-106">**사용자 편집** 페이지가 열리면 해당 사용자를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1db66-106">In the **Edit a user** page that opens, select the user.</span></span> <span data-ttu-id="1db66-107">사용자 속성 페이지가 열리면 **제품 라이선스**에 대 한 **편집** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="1db66-107">In the user properties page that opens, click **Edit** for **Product licenses**.</span></span>

3. <span data-ttu-id="1db66-108">**제품 라이선스** 페이지가 열리면 적절 한 **위치** 값을 선택 하 고 Exchange Online이 포함 된 라이선스 (세부 정보를 보려면 라이선스 확장)를 할당 합니다.</span><span class="sxs-lookup"><span data-stu-id="1db66-108">In the **Product licenses** page that opens, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="1db66-109">작업을 마쳤으면 **저장**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="1db66-109">When you're finished, click **Save**.</span></span>
