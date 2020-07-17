---
title: Yammer의 ID 정보
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146808"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="8832d-102">Yammer의 ID 정보</span><span class="sxs-lookup"><span data-stu-id="8832d-102">About identity in Yammer</span></span>

<span data-ttu-id="8832d-103">ID 관련 문제가 발생 하지 않도록 하려면 모든 네트워크에 다음 단계를 수행하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="8832d-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="8832d-104">모든 사용자가 기본 Microsoft 365 계정을 사용하여 로그인 하도록 Azure AD의 사용자에 대해 Microsoft 365 계정을 프로비전 한 후 Office 365 ID를 적용하세요.</span><span class="sxs-lookup"><span data-stu-id="8832d-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="8832d-105">자세한 내용은 [Yammer 사용자에 Office 365 ID 적용](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8832d-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="8832d-106">여러 Yammer 네트워크 통합</span><span class="sxs-lookup"><span data-stu-id="8832d-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="8832d-107">레거시 Yammer 구성에서는 여러 Yammer 네트워크를 하나의 테넌트로 연결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8832d-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="8832d-108">자세한 내용은 [네트워크 마이그레이션: 여러 Yammer 네트워크 통합](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8832d-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="8832d-109">Yammer 라이선스가 없는 사용자를 차단하기 위하여 Yammer 라이선스를 강제할 수 있는 옵션이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8832d-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="8832d-110">자세한 내용은 [Office 365에서 Yammer 사용자 라이선스 관리](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8832d-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="8832d-111">마지막으로, 이전 Yammer 네트워크의 사용자 목록을 감사하고 레거시 사용자를 일시 중단 합니다.</span><span class="sxs-lookup"><span data-stu-id="8832d-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="8832d-112">삭제를 취소할 수 없으므로 사용자를 삭제하는 대신 일시 중단 (비활성화)을 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="8832d-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="8832d-113">자세한 내용은 [Office 365에 연결된 네트워크에서 Yammer 사용자를 감사](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) 및 [사용자 삭제](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8832d-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="8832d-114">이 단계를 사용하여 Yammer를 구성하면 Microsoft 365의 기본 모드에서 Yammer 네트워크를 구성 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8832d-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="8832d-115">자세한 내용은 [Microsoft 365 기본 모드 Yammer 네트워크 구성](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8832d-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>