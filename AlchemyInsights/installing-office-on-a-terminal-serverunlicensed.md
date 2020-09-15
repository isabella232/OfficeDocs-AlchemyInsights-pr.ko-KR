---
title: 터미널 서버에 office 설치-사용 허가 되지 않음
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663123"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="f69fa-102">터미널 서버에 Office 설치</span><span class="sxs-lookup"><span data-stu-id="f69fa-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="f69fa-103">이전의 터미널 서비스를 사용 하 여 RDS (원격 데스크톱 서비스)를 사용한 Windows Server에 Microsoft 365 Apps for enterprise를 배포 하는 데 필요한 작업입니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="f69fa-104">Office 365 Enterprise E3 또는 Enterprise e 3과 같은 microsoft 365 앱 for enterprise를 포함 하는 Microsoft 365 구독이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="f69fa-105">Microsoft 365 비즈니스용 business 및 Microsoft 365 Apps Premium 요금제에는 Microsoft 365 앱 for enterprise가 포함 되어 있지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="f69fa-106">[공유 컴퓨터 활성화](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)를 사용 하도록 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="f69fa-107">Microsoft 365 관리 센터에서 RDS에 Microsoft 365 앱을 설치 하려면 ***기본 설치 설정을 사용 하는***경우에는 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="f69fa-108">[Microsoft 지원 및 복구 도우미](https://aka.ms/SaRA_OfficeSCA_M365Portal) 를 다운로드 하 고 실행 하 여 공유 컴퓨터 활성화 모드에서 Microsoft 365 Apps For enterprise office를 설치할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="f69fa-109">보유 하 고 있는 Microsoft 365 구독을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="f69fa-110">방법 알아보기</span><span class="sxs-lookup"><span data-stu-id="f69fa-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="f69fa-111">필요한 경우 다른 Microsoft 365 구독으로 전환 합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="f69fa-112">방법 알아보기</span><span class="sxs-lookup"><span data-stu-id="f69fa-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="f69fa-113">다른 Microsoft 365 구독을 사용 하 여 Office가 RDS 서버에 이미 설치 되어 있는 경우 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="f69fa-114">예를 들어 제어판으로 이동 하 여 \> 프로그램을 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="f69fa-115">문제가 발생 하는 경우 [Microsoft 지원 및 복구 도우미를](https://aka.ms/SARA-OfficeUninstall-Alchemy) 사용 하 여 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="f69fa-116">RDS 서버에서 관리자 계정으로 Microsoft 365 관리 센터에 로그인 하 고 [microsoft 365 앱 for enterprise를 설치](https://portal.office.com/OLS/MySoftware.aspx)합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="f69fa-117">Office를 설치한 후에는 열거나 Office 응용 프로그램에 ***로그인 하지 마세요*** .</span><span class="sxs-lookup"><span data-stu-id="f69fa-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="f69fa-118">RDS 서버에서 다음 단계를 수행 하 여 레지스트리를 편집 하 여 공유 컴퓨터 활성화를 사용 하도록 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="f69fa-119">화면 왼쪽 아래에 있는 Windows 단추를 마우스 오른쪽 단추로 클릭 하 고 실행을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="f69fa-120">열기 상자에 **regedit**를 입력 하 고 확인을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="f69fa-121">레지스트리 편집기를 사용 하 여 장치를 변경할 수 있는지 묻는 메시지가 표시 되 면 예를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="f69fa-122">레지스트리 편집기에서 HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.에 설정 1을 사용 하 여 **Sharedcomputerlicensing** 의 문자열 값을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="f69fa-123">RDS 서버에서 ***최종 사용자로 로그인*** 하 고 [Microsoft 365 for enterprise 앱에 대해 공유 컴퓨터 활성화가 사용 하도록 설정 되어 있는지 확인](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)합니다.</span><span class="sxs-lookup"><span data-stu-id="f69fa-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="f69fa-124">Office 배포 도구를 사용 하 여 필수 구성 요소, 설치 지침 및 사용자 지정 설치에 대 한 지침에 대 한 자세한 내용은 [Deploy Microsoft 365 Apps for enterprise for a Remote 데스크톱 Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="f69fa-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="f69fa-125">공유 컴퓨터 활성화와 관련 된 오류를 해결 하려면 [엔터프라이즈에 대 한 Microsoft 365 앱에 대 한 공유 컴퓨터 활성화의 문제 해결](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="f69fa-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  