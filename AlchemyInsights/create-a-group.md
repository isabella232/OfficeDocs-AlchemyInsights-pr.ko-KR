---
title: 그룹 만들기
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086392"
---
# <a name="create-a-group"></a><span data-ttu-id="5ea64-102">그룹 만들기</span><span class="sxs-lookup"><span data-stu-id="5ea64-102">Create a group</span></span>

<span data-ttu-id="5ea64-103">이 항목에서는 그룹 만들기에 대해 설명 합니다.</span><span class="sxs-lookup"><span data-stu-id="5ea64-103">This topic describes group creation.</span></span>

<span data-ttu-id="5ea64-104">**그룹을 만들 수 있는 권한**</span><span class="sxs-lookup"><span data-stu-id="5ea64-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="5ea64-105">새 그룹을 만들 수 있는 권한이 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="5ea64-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="5ea64-106">전역 관리자는 Azure portal 또는 Access 패널에서 그룹 만들기를 사용 하지 않도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5ea64-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="5ea64-107">관리자가 사용자를 위해 새 그룹을 만들거나 적절 한 사용 권한을 부여 해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5ea64-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="5ea64-108">**그룹 만들기 권한 관리**</span><span class="sxs-lookup"><span data-stu-id="5ea64-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="5ea64-109">전역 관리자는 **모든 그룹**  >  **일반 (설정)** 에서 "사용자가 azure portal에서 보안 그룹을 만들 수 있습니다." 또는 "사용자가 azure 포털에서 office 365 그룹을 만들 수 있습니다." 옵션을 선택 하 여 그룹 만들기 권한 (보안 관련 원인) 또는 office 365 그룹을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5ea64-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="5ea64-110">Azure Active Directory P1 Premium 라이선스가 있는 경우 그룹 만들기를 제한 하 여 사용자 그룹을 선택할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5ea64-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="5ea64-111">**새 Office 365 그룹 구성원에 대해 환영 알림을 사용 하지 않도록 설정**</span><span class="sxs-lookup"><span data-stu-id="5ea64-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="5ea64-112">Powershell에서 **UnifiedGroupWelcomeMessageEnabled** 를 False로 설정 하 여 Office 365 그룹에 추가 된 사용자에 게 전송 되는 환영 알림을 사용 하지 않도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5ea64-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="5ea64-113">이 [설정에](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)대해 자세히 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="5ea64-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

