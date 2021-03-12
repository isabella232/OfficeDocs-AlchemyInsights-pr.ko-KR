---
title: 액세스 거부 메시지 문제 해결
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707960"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="9cd6c-102">Sharepoint/OneDrive 관리 센터에서 액세스 거부 메시지 문제 해결</span><span class="sxs-lookup"><span data-stu-id="9cd6c-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="9cd6c-103">Sharepoint/OneDrive 관리 센터로 탐색하려고 할 때 액세스 거부 메시지가 수신된 경우 사용자에게 라이선스를 할당해야 [합니다.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="9cd6c-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="9cd6c-104">사용자에게 라이선스가 있는 경우 관리 센터에 [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) 액세스할 수 있는 관리자 역할이 할당되어 있는지도 확인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9cd6c-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="9cd6c-105">이 문제는 사용자가 삭제된 후 UPN(사용자 계정 이름)으로 다시 만들어질 때도 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cd6c-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="9cd6c-106">새 계정은 다른 PUID(Passport Unique ID) 값을 사용하여 만들어집니다.</span><span class="sxs-lookup"><span data-stu-id="9cd6c-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="9cd6c-107">사용자가 사이트 모음 또는 OneDrive에 액세스하면 사용자에게 잘못된 PUID가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cd6c-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="9cd6c-108">두 번째 시나리오에는 Active Directory OU(조직 구성 단위)와 디렉터리 동기화가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="9cd6c-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="9cd6c-109">사용자가 이미 SharePoint에 로그인한 후 다른 OU로 이동되어 SharePoint와 다시동기된 경우 이 문제가 발생하게 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cd6c-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="9cd6c-110">이 문제를 해결하기 위해 [Microsoft 365에서](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)사용자 복원 문서의 단계를 통해 원래 UPN을 복원해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9cd6c-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="9cd6c-111">참고: 이전에 액세스한 여러 사용자가 OneDrive 또는 SharePoint 관리 센터를 사용할 수 없는 경우 일시적인 서비스 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cd6c-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="9cd6c-112">[서비스 상태 대시보드를 선택합니다.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="9cd6c-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


