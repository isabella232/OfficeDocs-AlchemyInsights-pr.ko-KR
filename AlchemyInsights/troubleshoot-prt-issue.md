---
title: PRT 문제 해결
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571971"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="36cd4-102">PRT 문제 해결</span><span class="sxs-lookup"><span data-stu-id="36cd4-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="36cd4-103">인증을 완료하려면 장치가 완전히 등록되어 있으며 양호한 상태로 PRT(기본 새로 고침 토큰)를 획득할 수 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="36cd4-104">하이브리드 Azure AD 가입 등록 프로세스를 사용하려면 장치가 회사 네트워크에 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="36cd4-105">또한 VPN을 통해 작동하지만 몇 가지 주의가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="36cd4-106">고객이 원격 작업 환경에서 하이브리드 Azure AD 가입 등록 프로세스 문제 해결에 도움이 필요하다는 소식을 들었을 것입니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="36cd4-107">다음은 등록 프로세스 중에 '후드 아래'에서 진행된 일에 대한 분석입니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="36cd4-108">**클라우드 인증 환경(Azure AD 암호 해시 동기화 또는 통과 인증 사용)**</span><span class="sxs-lookup"><span data-stu-id="36cd4-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="36cd4-109">이 등록 흐름을 "동기화 참가"라고도 합니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="36cd4-110">Windows 10은 사용자가 장치에 로그온할 때 SCP 레코드를 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="36cd4-111">장치는 먼저 레지스트리 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]에서 클라이언트 쪽 SCP에서 테넌트 정보를 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="36cd4-112">자세한 내용은 이 [문서를](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="36cd4-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="36cd4-113">오류가 발생하면 장치가 SCP(서비스 연결 지점)에서 테넌트 정보를 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="36cd4-114">SCP를 확인한 후 이 문서를 [참조합니다.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)</span><span class="sxs-lookup"><span data-stu-id="36cd4-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="36cd4-115">AD에서 SCP를 사용하도록 설정하고 초기 유효성 검사를 위해 클라이언트 쪽 SCP만 사용하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="36cd4-116">Windows 10은 시스템 컨텍스트에서 Azure AD와 통신하여 Azure AD에 대해 인증을 합니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="36cd4-117">장치 등록 연결 테스트 스크립트를 사용하여 장치가 시스템 계정의 Microsoft 리소스에 액세스할 수 있는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="36cd4-118">Windows 10은 자체 서명된 인증서를 생성하고 이 인증서를 컴퓨터 개체 아래에 On-premises AD에 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="36cd4-119">이를 위해서는 도메인 컨트롤러에 대한 시야가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="36cd4-120">인증서가 있는 장치 개체는 Azure AD Connect를 통해 Azure AD에 동기화됩니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="36cd4-121">동기화 주기는 기본적으로 30분마다 마다 되지만 Azure AD Connect의 구성에 따라 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="36cd4-122">자세한 내용은 이 문서를 [참조하세요.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)</span><span class="sxs-lookup"><span data-stu-id="36cd4-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="36cd4-123">이 단계에서 Azure Portal의 장치 블레이드에서 "보류 중" 상태로 주체 장치를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="36cd4-124">다음에 Windows 10에 로그인하면 등록이 완료됩니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="36cd4-125">VPN을 사용 중일 때 로그프 로그인 프로세스로 도메인 연결이 종료되는 경우 등록을 수동으로 트리거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="36cd4-126">관리자 프롬프트에서 로컬로 또는 PSExec을 통해 PC에 원격으로 dsregcmd /join을 발급합니다.</span><span class="sxs-lookup"><span data-stu-id="36cd4-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="36cd4-127">예: PsExec -s \\ win10client01 cmd, dsregcmd /join</span><span class="sxs-lookup"><span data-stu-id="36cd4-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="36cd4-128">하이브리드 가입 문제에 대한 자세한 내용은 장치 문제 [해결을 참조합니다.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)</span><span class="sxs-lookup"><span data-stu-id="36cd4-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
