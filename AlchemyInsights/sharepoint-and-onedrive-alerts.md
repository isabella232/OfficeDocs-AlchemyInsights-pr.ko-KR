---
title: SharePoint 및 OneDrive 경고 수신 지연
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: fd00bd90de382e325a9b8c4ce5b21d535e630730
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831236"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="e6f33-102">SharePoint 및 OneDrive 경고 수신 지연</span><span class="sxs-lookup"><span data-stu-id="e6f33-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="e6f33-103">여러 **파일 또는** 라이브러리의 모든 경고가 지연되는 경우 [서비스](https://portal.office.com/adminportal/home?ref=/servicehealth) 상태 대시보드를 방문하여 SharePoint 또는 Exchange에서 발생될 수 있는 권고/인시던트가 없는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e6f33-103">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span>
- <span data-ttu-id="e6f33-104">특정 **파일 또는** 라이브러리의 개별 경고가 배달되지 않은 경우 삭제한 후 다시 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="e6f33-104">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="e6f33-105">경고를 다시 생성하려면 SharePoint 경고 [관리,](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) 보기 또는 삭제를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="e6f33-105">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="e6f33-106">전자 메일에서 정크 또는 스팸 폴더를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="e6f33-106">Check the Junk or Spam folder in your email.</span></span>

> [!NOTE]
> - <span data-ttu-id="e6f33-107">경고를 메일 그룹으로 보낼 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="e6f33-107">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="e6f33-108">보안 및 O365 그룹만 지원됩니다.</span><span class="sxs-lookup"><span data-stu-id="e6f33-108">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="e6f33-109">경고 전자 메일 서식 파일은 사용자 지정할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="e6f33-109">You cannot customize alert email templates.</span></span> <span data-ttu-id="e6f33-110">이러한 작업을 위해서는 Microsoft Flow 또는 SharePoint Designer 워크플로를 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e6f33-110">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
