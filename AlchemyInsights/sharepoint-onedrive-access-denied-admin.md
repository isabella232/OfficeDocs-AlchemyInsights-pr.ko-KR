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
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767668"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="3534b-102">Sharepoint/OneDrive 관리 센터에서 액세스 거부 메시지 문제 해결</span><span class="sxs-lookup"><span data-stu-id="3534b-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="3534b-103">Sharepoint/OneDrive 관리 센터를 탐색 하려고 할 때 액세스 거부 메시지가 표시 되는 경우 [사용자에 게 라이선스를 할당](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)했는지 확인 하세요.</span><span class="sxs-lookup"><span data-stu-id="3534b-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="3534b-104">사용자에 게 라이선스가 있는 경우 관리 센터에 액세스할 수 있는 [관리자 역할이 할당](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) 되었는지도 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3534b-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="3534b-105">동일한 UPN (사용자 계정 이름)을 사용 하 여 삭제 하 고 다시 만든 경우에도이 문제가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3534b-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="3534b-106">새 계정은 다른 PUID (Passport 고유 ID) 값을 사용 하 여 만들어집니다.</span><span class="sxs-lookup"><span data-stu-id="3534b-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="3534b-107">사용자가 사이트 모음 또는 OneDrive에 액세스 하려고 하면 사용자에 게 잘못 된 PUID가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3534b-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="3534b-108">두 번째 시나리오에는 Active Directory OU (조직 구성 단위)와의 디렉터리 동기화가 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3534b-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="3534b-109">사용자가 이미 SharePoint에 로그인 한 후 다른 OU로 이동 하 고 SharePoint를 사용 하 여 resynced이 문제가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3534b-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="3534b-110">이 문제를 해결 하려면 [Microsoft 365에서 사용자 복원](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)문서의 단계와 함께 원래 UPN을 복원 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3534b-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="3534b-111">참고: 이전에 액세스 한 여러 사용자가 OneDrive 또는 SharePoint 관리 센터를 사용할 수 없는 경우 일시적인 서비스 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3534b-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="3534b-112">[서비스 상태 대시보드를 확인](https://portal.office.com/adminportal/home#/servicehealth)합니다.</span><span class="sxs-lookup"><span data-stu-id="3534b-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


