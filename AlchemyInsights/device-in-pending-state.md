---
title: 보류 중인 상태의 장치
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652190"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="c3fd5-102">보류 중인 상태의 장치</span><span class="sxs-lookup"><span data-stu-id="c3fd5-102">Device in pending state</span></span>

<span data-ttu-id="c3fd5-103">**선행 사항:**</span><span class="sxs-lookup"><span data-stu-id="c3fd5-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="c3fd5-104">처음으로 장치 등록을 설정하는 경우 [Azure AD(Azure Active](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) Directory)의 장치 관리 소개를 검토하여 Azure AD를 통해 디바이스를 다운로드하는 방법을 안내합니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="c3fd5-105">장치를 Azure AD에 직접 등록하고 Intune에 등록하는 경우 [Intune을](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) 구성하고 라이선스를 먼저 [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="c3fd5-106">Azure AD 및 On-premises AD에서 작업을 수행할 수 있는 권한이 부여되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="c3fd5-107">Azure AD의 전역 관리자만 장치 등록에 대한 설정을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="c3fd5-108">또한 자동 등록을 설정하는 경우 Active Directory 및 AD FS의 관리자(해당되는 경우)를 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="c3fd5-109">하이브리드 Azure AD 가입 등록 프로세스를 사용하려면 장치가 회사 네트워크에 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="c3fd5-110">또한 VPN을 통해 작동하지만 몇 가지 주의가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="c3fd5-111">고객이 원격 작업 환경에서 하이브리드 Azure AD 가입 등록 프로세스 문제 해결에 도움이 필요하다는 소식을 들었을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="c3fd5-112">**클라우드 인증 환경(Azure AD 암호 해시 동기화 또는 통과 인증 사용)**</span><span class="sxs-lookup"><span data-stu-id="c3fd5-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="c3fd5-113">이 등록 흐름을 "동기화 참가"라고도 합니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="c3fd5-114">다음은 등록 프로세스 중에 발생하는 일에 대한 분석입니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="c3fd5-115">Windows 10은 사용자가 장치에 로그온할 때 SCP(서비스 연결 지점) 레코드를 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="c3fd5-116">장치는 먼저 레지스트리 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]에서 클라이언트 쪽 SCP에서 테넌트 정보를 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="c3fd5-117">자세한 내용은 문서를 [참조하십시오.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)</span><span class="sxs-lookup"><span data-stu-id="c3fd5-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="c3fd5-118">오류가 발생하면 장치가 SCP에서 테넌트 정보를 얻기 위해 On-premises Active Directory와 통신합니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="c3fd5-119">SCP를 확인하면 이 문서를 [참조합니다.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)</span><span class="sxs-lookup"><span data-stu-id="c3fd5-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="c3fd5-120">Active Directory에서 SCP를 사용하도록 설정하고 초기 유효성 검사에는 클라이언트 쪽 SCP만 사용하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="c3fd5-121">Windows 10은 시스템 컨텍스트에서 Azure AD와 통신하여 Azure AD에 대해 인증을 합니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="c3fd5-122">장치 등록 연결 테스트 스크립트를 사용하여 장치가 시스템 계정의 Microsoft 리소스에 액세스할 수 있는지 [확인할 수 있습니다.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)</span><span class="sxs-lookup"><span data-stu-id="c3fd5-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="c3fd5-123">Windows 10은 자체 서명된 인증서를 생성하고 컴퓨터 개체 아래에 해당 인증서를 등록된 Active Directory에 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="c3fd5-124">이를 위해서는 도메인 컨트롤러에 대한 시야가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="c3fd5-125">인증서가 있는 장치 개체는 Azure AD Connect를 통해 Azure AD에 동기화됩니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="c3fd5-126">동기화 주기는 기본적으로 30분마다 마다 되지만 Azure AD Connect의 구성에 따라 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="c3fd5-127">자세한 내용은 이 [문서를](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="c3fd5-128">이 단계에서는 Azure Portal의 장치 블레이드에서 **"보류** 중인" 상태의 주체 장치를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="c3fd5-129">다음에 Windows 10에 로그인하면 등록이 완료됩니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c3fd5-130">VPN을 사용 중일 때 로그프/로그인이 도메인 연결을 종료하는 경우 수동으로 등록을 트리거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="c3fd5-131">이를 위해</span><span class="sxs-lookup"><span data-stu-id="c3fd5-131">To do that:</span></span>
    >
    > <span data-ttu-id="c3fd5-132">관리자 `dsregcmd /join` 프롬프트에서 로컬로 발급하거나 PSExec을 통해 PC로 원격으로 발급합니다.</span><span class="sxs-lookup"><span data-stu-id="c3fd5-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="c3fd5-133">예: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="c3fd5-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="c3fd5-134">Azure Active Directory 장치 등록과 관련한 일반적인 문제는 [장치 FAQ를 참조하세요.](https://docs.microsoft.com/azure/active-directory/devices/faq)</span><span class="sxs-lookup"><span data-stu-id="c3fd5-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
