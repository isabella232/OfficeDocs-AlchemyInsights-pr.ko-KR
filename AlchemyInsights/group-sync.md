---
title: 그룹 동기화
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243924"
---
# <a name="group-sync"></a><span data-ttu-id="bb671-102">그룹 동기화</span><span class="sxs-lookup"><span data-stu-id="bb671-102">Group sync</span></span>

<span data-ttu-id="bb671-103">이 문서는 그룹 동기화에 대한 지침을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="bb671-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="bb671-104">전역 관리자 그룹 소유자가 그룹 속성을 수정하거나 Azure 포털에서 구성원을 추가하거나 소유자를 할당할 수 없는 경우 그룹의 권한이 글로벌 관리자 또는 그룹 소유자가 그룹을 수정할 수 있는 Azure Active Directory(Azure AD)인지 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="bb671-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="bb671-105">Azure AD에서 동기화된 그룹을 삭제하기 전에 먼저 오류 발생을 방지하기 위해 [할당된 모든 라이선스를 삭제](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced)했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="bb671-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="bb671-106">사용자, 그룹 및 연락처를 동기화하는 방법을 이해하기 위해 [Azure AD Connect 동기화](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)를 참조하고 [Azure AD Connect를 사용하여 Azure와 Azure 동기화](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support)를 따라 AD connect를 사용해 온-프레미스 그룹을 동기화하세요.</span><span class="sxs-lookup"><span data-stu-id="bb671-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="bb671-107">[동기화 중에 발생하는 오류 해결](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors)에 대한 이 지침에 따라 동기화 중에 발생하는 일반적인 오류를 해결하세요.</span><span class="sxs-lookup"><span data-stu-id="bb671-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

