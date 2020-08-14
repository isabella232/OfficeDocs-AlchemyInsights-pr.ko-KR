---
title: Office 앱에 대한 업데이트 채널 변경
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: fb69bce40ab56b162c715af6a0647c8219c5564f
ms.sourcegitcommit: dab885f2cb99057e959fb9be334f5a3a26a64058
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2020
ms.locfileid: "46665468"
---
# <a name="change-update-channels-for-office-apps"></a><span data-ttu-id="4ea1c-102">Office 앱에 대한 업데이트 채널 변경</span><span class="sxs-lookup"><span data-stu-id="4ea1c-102">Change update channels for Office apps</span></span>

<span data-ttu-id="4ea1c-103">새 Office 설치의 경우, Office 소프트웨어 다운로드 설정을 사용하여 원하는 업데이트 채널을 선택하고 Office 앱을 설치(또는 다시 설치)합니다.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-103">For new Office installations, use Office Software Download Settings to select the desired update channel, and then install (or re-install) Office apps.</span></span> <span data-ttu-id="4ea1c-104">자세한 내용은 [Office 365에서 소프트웨어 다운로드 설정 관리](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-104">For more info, see [Manage software download settings in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span></span> 

<span data-ttu-id="4ea1c-105">**참고** Office 소프트웨어 다운로드 설정을 사용하여 선택한 업데이트 채널은 O365 포털을 사용하여 새 설치를 수행하는 모든 사용자에게 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-105">**Note** The update channel selected using the Office Software Download Settings applies to all users performing new installations using the O365 portal.</span></span> <span data-ttu-id="4ea1c-106">자세한 내용은 [PC 또는 Mac에서 Microsoft 365 또는 Office 2019 다운로드 및 설치 또는 다시 설치](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-106">For more info, see [Download and install or reinstall Microsoft 365 or Office 2019 on a PC or Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span></span>   

<span data-ttu-id="4ea1c-107">기존 Office 설치의 경우, ODT(Office Deployment Tool)를 사용하여 다른 업데이트 채널로 전환합니다.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-107">For existing Office installations, use the Office Deployment Tool (ODT) to switch to a different update channel:</span></span>  

1. <span data-ttu-id="4ea1c-108">[Microsoft 다운로드 센터](https://go.microsoft.com/fwlink/p/?LinkID=626065)에서 Office 배포 도구(setup.exe)의 최신 버전을 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-108">Download the latest version of the Office Deployment Tool (setup.exe) from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
2. <span data-ttu-id="4ea1c-109">전환하려는 채널의 이름을 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-109">Identify the name of the channel that you want to switch to.</span></span> <span data-ttu-id="4ea1c-110">자세한 내용은 [Office 배포 도구에 대한 구성 옵션](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-110">For more info, see [Configuration options for the Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span></span>
3. <span data-ttu-id="4ea1c-111">적절한 채널 이름(예: update.exe)을 지정하여 구성 XML 파일을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-111">Create a configuration XML file specifying the appropriate channel name, for example, update.xml.</span></span>  
    `<Configuration> 
    <Updates **Channel="Monthly"** />  
    </Configuration>`
4. <span data-ttu-id="4ea1c-112">관리자 권한으로 실행한 명령 프롬프트에서 setup.exe가 있는 폴더 위치로 전환하고 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-112">From an elevated command prompt, switch to the folder location where setup.exe resides and run the following command:</span></span>  
    <span data-ttu-id="4ea1c-113">a.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-113">a.</span></span> <span data-ttu-id="4ea1c-114">setup.exe /configure update.xml</span><span class="sxs-lookup"><span data-stu-id="4ea1c-114">setup.exe /configure update.xml</span></span>
5. <span data-ttu-id="4ea1c-115">Excel과 같은 Office 응용 프로그램을 시작한 다음 **파일** > **계정**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-115">Start an Office application (such as Excel), and then select **File** > **Account**.</span></span> <span data-ttu-id="4ea1c-116">제품 정보 섹션에서 **업데이트 옵션** > **지금 업데이트**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-116">In the Product Information section, select **Update Options** > **Update Now**.</span></span>

<span data-ttu-id="4ea1c-117">자세한 내용은 [기존 Office 앱에 대한 업데이트 채널을 전환하는 방법](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-117">For more information, see [How to switch update channels for existing Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span></span> 

<span data-ttu-id="4ea1c-118">선택한 사용자 그룹에 대한 업데이트 채널을 전환하거나 SCCM(System Center Configuration Manager)을 사용하여 전환하는 경우 GPO를 사용하여 업데이트 채널 설정을 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-118">For switching update channels for a selected group of users or by using Configuration Manager (SCCM), configure the Update Channel setting using GPO.</span></span> <span data-ttu-id="4ea1c-119">자세한 내용은 [Microsoft 365 앱의 업데이트 채널 개요](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-119">For more info, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span></span> <span data-ttu-id="4ea1c-120">자세한 내용은 [IT 전문가용 Office 365 ProPlus 채널을 관리하는 방법](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) 및 [Microsoft Configuration Manager를 사용하여 Microsoft 365 앱에 대한 업데이트를 관리하는 방법](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="4ea1c-120">For details, see [How to manage Office 365 ProPlus Channels for IT Pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) and [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span></span>