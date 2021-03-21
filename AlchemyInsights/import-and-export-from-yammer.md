---
title: Yammer에서 가져오기 및 내보내기
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898051"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="e5c62-102">Yammer에서 가져오기 및 내보내기</span><span class="sxs-lookup"><span data-stu-id="e5c62-102">Import and export from Yammer</span></span>

<span data-ttu-id="e5c62-103">**가져오기**</span><span class="sxs-lookup"><span data-stu-id="e5c62-103">**Import**</span></span>

<span data-ttu-id="e5c62-104">사용자 가져오기 옵션은 Yammer 네트워크가 [Microsoft 365의 기본 모드](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode) 상태인지 여부에 따라 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="e5c62-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="e5c62-105">**기본이 아닌 모드**: 사용자는 [주소록에서 추가](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294)를 사용하여 그룹 설정 내에서 (사용자 100명 이내로 제한) 그룹으로 가져오거나 네트워크 관리자 내에서 [일괄 업데이트](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users)를 사용하여 네트워크로 가져올 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e5c62-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="e5c62-106">**기본 모드**: 그룹 멤버 자격 및 네트워크 멤버 자격 작업은 [Microsoft 365 관리 포털](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD 포털](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)또는 다른 Azure AD 옵션을 사용하여 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e5c62-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="e5c62-107">기본 모드의 네트워크에서는 더 이상 대량 업데이트 및 기타 레거시 기능에 액세스할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="e5c62-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e5c62-108">데이터 내보내기 기능이 다른 네트워크에서 사용된 경우에도 Yammer는 네트워크 관리자 내에서 콘텐츠 가져오기 기능을 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="e5c62-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="e5c62-109">콘텐츠는 파트너 솔루션 또는 Yammer REST API에 의해 다시 게시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e5c62-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="e5c62-110">**내보내기**</span><span class="sxs-lookup"><span data-stu-id="e5c62-110">**Export**</span></span>

<span data-ttu-id="e5c62-111">[네트워크 관리 센터 내에서 네트워크 내보내기](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data)는 메시지 및 파일을 포함하여 Yammer 네트워크에서 콘텐츠 내보내기를 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="e5c62-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="e5c62-112">첨부 파일이 매우 크면 내보내기 완료에 상당한 시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e5c62-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="e5c62-113">활성 네트워크는 일 또는 주 단위로 [데이터 내보내기 API](https://developer.yammer.com/docs/data-export-api)를 사용하여 내보내는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="e5c62-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="e5c62-114">Microsoft 지원에서는 이러한 용도로 사용자 지정 스크립트를 제공하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="e5c62-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="e5c62-115">별도의 [ GDPR 내보내기](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise)는 개별 사용자를 위한 콘텐츠를 내보내기 위해 존재합니다.</span><span class="sxs-lookup"><span data-stu-id="e5c62-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>