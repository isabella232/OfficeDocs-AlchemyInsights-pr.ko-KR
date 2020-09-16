---
title: RDS, 터미널 서버 또는 VDI에서 공유 하기 위한 Microsoft 365 Apps for enterprise 배포
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 22ded616e82b2e82023b55a1d3ca6251cfb71712
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745541"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="556f7-102">RDS, 터미널 서버 또는 VDI에서 공유 하기 위한 Microsoft 365 Apps for enterprise 배포</span><span class="sxs-lookup"><span data-stu-id="556f7-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="556f7-103">RDS (원격 데스크톱 서비스)를 사용 하 여 기업에 대 한 Microsoft 365 앱 (이전의 터미널 서비스)을 배포 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="556f7-104">Office 365 Enterprise E3 또는 Enterprise e 5와 같이 microsoft 365 For enterprise for Business 요금제 또는 Office 365 요금제를 포함 해야 365 합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="556f7-105">Microsoft 365 비즈니스용 business 및 Microsoft 365 Business Premium Standard 요금제에는 Microsoft 365 앱 for enterprise가 포함 되어 있지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-105">The Microsoft 365 Apps for business and Microsoft 365 Business Premium Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="556f7-106">[공유 컴퓨터 활성화](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)를 사용 하도록 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="556f7-107">[Microsoft 지원 및 복구 도우미](https://aka.ms/SaRA_OfficeSCA_M365Portal) 를 다운로드 하 고 실행 하 여 공유 컴퓨터 활성화 모드에서 Microsoft 365 Apps For enterprise office를 설치할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="556f7-108">Office 배포 도구를 사용 하 여 필수 구성 요소, 설치 지침 및 사용자 지정 설치 지침에 대 한 자세한 내용은 [원격 데스크톱 서비스를 사용 하 여 엔터프라이즈 용 Microsoft 365 앱 배포](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="556f7-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="556f7-109">공유 컴퓨터 활성화와 관련 된 오류를 해결 하려면</span><span class="sxs-lookup"><span data-stu-id="556f7-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="556f7-110">[엔터프라이즈에 대 한 Microsoft 365 앱에 대 한 공유 컴퓨터 정품 인증과 관련 된 문제 해결을](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="556f7-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="556f7-111">[엔터프라이즈용 Microsoft 365 앱 정품인증 재설정](https://go.microsoft.com/fwlink/?linkid=2109218)을 참고하세요.</span><span class="sxs-lookup"><span data-stu-id="556f7-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="556f7-112">***기본 설치 설정을 사용 하는***microsoft 365 관리 센터에서 RDS에 Microsoft 365 Apps for enterprise를 설치 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.    <span data-ttu-id="556f7-113">보유 하 고 있는 구독을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-113">Check what subscription you have.</span></span> <span data-ttu-id="556f7-114">[방법을 알아보세요](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="556f7-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.    <span data-ttu-id="556f7-115">필요한 경우 다른 구독으로 전환 합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="556f7-116">[방법을 알아보세요](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="556f7-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3.    <span data-ttu-id="556f7-117">다른 Microsoft 구독을 사용 하 여 Office가 이미 RDS 서버에 설치 되어 있는 경우 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="556f7-118">예를 들어 **제어판**으로 이동 하 여  >  **프로그램을 제거**합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="556f7-119">문제가 발생 하는 경우 [Microsoft 지원 및 복구 도우미를](https://aka.ms/SARA-OfficeUninstall-Alchemy) 사용 하 여 제거 합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.    <span data-ttu-id="556f7-120">RDS 서버에서 관리자 계정으로 Microsoft 365 관리 센터에 로그인 하 고 [microsoft 365 앱 for enterprise를 설치](https://portal.office.com/OLS/MySoftware.aspx)합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.    <span data-ttu-id="556f7-121">Office를 설치한 후에는 열거나 Office 응용 프로그램에 ***로그인 하지 마세요*** .</span><span class="sxs-lookup"><span data-stu-id="556f7-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.    <span data-ttu-id="556f7-122">RDS 서버에서 다음 단계를 수행 하 여 레지스트리를 편집 하 여 공유 컴퓨터 활성화를 사용 하도록 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="556f7-123">화면 왼쪽 아래 모서리에 있는 Windows 단추를 마우스 오른쪽 단추로 클릭 하 고 **실행**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="556f7-124">열기 상자에 **regedit**를 입력 하 고 **확인**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="556f7-125">레지스트리 편집기를 사용 하 여 장치를 변경할 수 있는지 묻는 메시지가 표시 되 면 **예** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="556f7-126">레지스트리 편집기에서 HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.에 설정 1을 사용 하 여 **Sharedcomputerlicensing** 의 문자열 값을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="556f7-127">RDS 서버에서 ***최종 사용자로 로그인*** 하 고 [Microsoft 365 for enterprise 앱에 대해 공유 컴퓨터 활성화가 사용 하도록 설정 되어 있는지 확인](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)합니다.</span><span class="sxs-lookup"><span data-stu-id="556f7-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

