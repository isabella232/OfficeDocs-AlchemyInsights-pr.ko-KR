---
title: OneDrive 동기화 클라이언트의 조직 이름 변경
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003077"
- "5850"
ms.openlocfilehash: ca545ba51e39209f3302acdee1c24048515e2c1b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818330"
---
# <a name="change-the-organization-name-for-the-onedrive-sync-client"></a><span data-ttu-id="1dbfc-102">OneDrive 동기화 클라이언트의 조직 이름 변경</span><span class="sxs-lookup"><span data-stu-id="1dbfc-102">Change the organization name for the OneDrive sync client</span></span>

<span data-ttu-id="1dbfc-103">OneDrive에서는 테넌트 관리자가 설정한 회사 이름을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="1dbfc-103">OneDrive uses the organization name set by a tenant administrator.</span></span>  <span data-ttu-id="1dbfc-104">[조직 주소, 기술 담당자 등을 변경](https://docs.microsoft.com/microsoft-365/admin/manage/change-address-contact-and-more)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1dbfc-104">You can [change your organization's address, technical contact, and more](https://docs.microsoft.com/microsoft-365/admin/manage/change-address-contact-and-more).</span></span> <span data-ttu-id="1dbfc-105">해당 변경 내용이 테넌트에 대해 수행되면 OneDrive 동기화 클라이언트에서 사용자가 OneDrive 계정을 연결을 끊은 후 다시 연결할 때까지 새 이름을 반영하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1dbfc-105">Once that change is performed for the tenant, the OneDrive sync client will not reflect the new name until users unlink and relink their OneDrive account.</span></span>

<span data-ttu-id="1dbfc-106">계정 연결을 끊으려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="1dbfc-106">To unlink the account:</span></span>

1. <span data-ttu-id="1dbfc-107">작업 표시줄의 맨 오른쪽에 있는 파란색 OneDrive 구름 아이콘을 선택한 다음, **추가 > 설정 > 계정** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1dbfc-107">Select the blue OneDrive cloud icon at the far right of the taskbar, then select  **More > Settings > Account**.</span></span>
2. <span data-ttu-id="1dbfc-108">링크를 끊을 계정을 찾은 다음 **이 PC 연결 끊기** 를 선택한 후 **계정 연결 끊기** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1dbfc-108">Find the account you want to unlink and select  **Unlink this PC**, and then  **Unlink account**.</span></span>

<span data-ttu-id="1dbfc-109">계정을 다시 연결하려면 설정의 **계정** 탭에서 **계정 추가** 를 선택하고 OneDrive에 다시 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="1dbfc-109">To relink the account, select  **Add an account** from the  **Account** tab in Settings, and sign back into OneDrive.</span></span>