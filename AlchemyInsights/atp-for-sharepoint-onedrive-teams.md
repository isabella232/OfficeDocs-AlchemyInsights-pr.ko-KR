---
title: SharePoint, OneDrive 및 Microsoft Teams에 대한 ATP
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508418"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="c48a4-102">SharePoint, OneDrive 및 Microsoft Teams에 대한 ATP</span><span class="sxs-lookup"><span data-stu-id="c48a4-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="c48a4-103">Advanced Threat Protection을 사용 하도록 설정 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="c48a4-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="c48a4-104">로 이동 하 [https://protection.office.com](https://protection.office.com) 고 전역 관리자 또는 보안 관리자 계정으로 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c48a4-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="c48a4-105">왼쪽 탐색 창의 **위협 관리**에서 **정책** \> **안전한 첨부 파일**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c48a4-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="c48a4-106">**SharePoint, OneDrive 및 Microsoft 팀에 대해 ATP 사용**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c48a4-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="c48a4-107">악의적인 파일을 검색할 때 알림을 수신 하 [는 작업 경고 정책을 만듭니다](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) .</span><span class="sxs-lookup"><span data-stu-id="c48a4-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="c48a4-108">자세한 내용은이 [항목](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="c48a4-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="c48a4-109">**참고**: ATP은 SharePoint Online, 비즈니스용 OneDrive 또는 Microsoft 팀에서 모든 단일 파일을 검색 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c48a4-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="c48a4-110">파일은 공유 작업, 게스트 작업 및 위협 신호를 사용 하 여 악성 파일을 식별 하는 프로세스에서 비동기적으로 검색 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c48a4-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="c48a4-111">자세한 내용은이 [항목](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="c48a4-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
