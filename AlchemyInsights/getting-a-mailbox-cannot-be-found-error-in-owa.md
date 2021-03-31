---
title: 126 OWA에서 사서함을 찾을 수 없는 경우
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426668"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="43230-102">웹에서 Outlook에서 사서함을 찾을 수 없는 오류 발생</span><span class="sxs-lookup"><span data-stu-id="43230-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="43230-103">웹용 Outlook을 사용 중일 때  오류로 사서함을 찾을 수 없는 경우 웹용 Outlook에 연결하는 데 사용한 계정에 Exchange Online 라이선스가 없습니다. 따라서 사서함이 계정과 연결되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="43230-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="43230-104">관리자는 다음 단계에 따라 계정에 라이선스를 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43230-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="43230-105">Microsoft [365](https://portal.office.com/adminportal/home#/homepage) 관리 센터를  열고 사용자  섹션에서 활성 사용자로 이동한 다음 오류가 표시하는 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="43230-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="43230-106">열 수 있는 사용자 페이지에서 라이선스  및 앱 섹션으로 이동하여 적절한 위치 값을 선택한 다음 Exchange Online이 포함된 라이선스를 할당합니다(라이선스를 확장하여 세부 정보를 확인). </span><span class="sxs-lookup"><span data-stu-id="43230-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="43230-107">작업을 마쳤으면 **변경 내용 저장** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="43230-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="43230-108">경우에 따라 라이선스가 사용자 계정에 이미 할당된 경우 라이선스를 제거하고 다시 할당하면 문제를 해결하고 시스템에 올바르게 프로비전하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="43230-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="43230-109">M365 Exchange Online 및 기타(있는 경우) 구독이 현재 있으며 최근에 만료되지 않은지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43230-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="43230-110">구독이 만료되지 않고 유효한 라이선스가 사용자 계정에 할당된 경우 라이선스가 프로비전되는 데 최대 24시간이 걸릴 수 있으므로 문제가 해결될 때까지 기다려야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43230-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="43230-111">자세한 내용은 라이선스 할당 및 [관리를 참조하세요.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="43230-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>