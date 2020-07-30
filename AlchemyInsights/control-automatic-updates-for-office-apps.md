---
title: Office 앱에 대한 자동 업데이트 제어
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431620"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="bde5b-102">Office 앱에 대한 자동 업데이트 제어</span><span class="sxs-lookup"><span data-stu-id="bde5b-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="bde5b-103">기본적으로 Office 앱에 대한 업데이트는 자동으로 다운로드되어 사용자 개입 없이 백그라운드에서 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="bde5b-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="bde5b-104">그러나 관리자는 Office 업데이트 설정을 사용하여 업데이트를 적용하는 방법을 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bde5b-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="bde5b-105">업데이트 설정을 사용하면 관리자가 자동 업데이트를 사용하거나 사용하지 않도록 설정하고, Office에서 **지금 업데이트** 단추를 표시하거나 숨기고, 업데이트 마감일을 설정하는 등 다양한 작업을 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bde5b-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="bde5b-106">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="bde5b-106">For detailed information, see:</span></span>

- [<span data-ttu-id="bde5b-107">Office의 업데이트 설정 구성</span><span class="sxs-lookup"><span data-stu-id="bde5b-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="bde5b-108">Office의 자동 업데이트를 사용할 수 없음</span><span class="sxs-lookup"><span data-stu-id="bde5b-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="bde5b-109">설치 후 Office를 업데이트하는 방법 정의</span><span class="sxs-lookup"><span data-stu-id="bde5b-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="bde5b-110">클라이언트 머신에 적용된 기존 업데이트 설정을 검토하려면 다음 단계를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="bde5b-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="bde5b-111">**시작** > **실행** > **regedit**로 이동하여 레지스트리 편집기를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="bde5b-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="bde5b-112">다음 위치로 전환하고 Office 업데이트 설정을 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="bde5b-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="bde5b-113">a.</span><span class="sxs-lookup"><span data-stu-id="bde5b-113">a.</span></span> <span data-ttu-id="bde5b-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="bde5b-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="bde5b-115">b.</span><span class="sxs-lookup"><span data-stu-id="bde5b-115">b.</span></span> <span data-ttu-id="bde5b-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="bde5b-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="bde5b-117">**참고**  OfficeMgmtCOM 키가 설정되어 있는 경우 **Office** > **계정** > **Office 업데이트**에 "업데이트는 시스템 관리자가 관리합니다."라는 메시지가 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bde5b-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="bde5b-118">자세한 내용은 [Microsoft Endpoint Configuration Manager를 사용하여 Microsoft 365 앱으로의 업데이트 관리하기](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="bde5b-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  