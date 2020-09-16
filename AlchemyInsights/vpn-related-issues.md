---
title: VPN 관련 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726097"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="b2fb4-102">VPN 관련 문제</span><span class="sxs-lookup"><span data-stu-id="b2fb4-102">VPN related issues</span></span>

<span data-ttu-id="b2fb4-103">MDM 클라이언트용 VPN 연결의 성공적인 구현은 VPN 인프라의 요구 사항을 올바르게 반영하는 배포 된 프로필에 따라 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="b2fb4-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="b2fb4-104">조사 중인 클라이언트 플랫폼의 적절한 설정은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b2fb4-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="b2fb4-105">Intune을 사용하여 VPN 연결을 추가하기 위해 Windows 10 및 Windows 홀로그램 장치 설정</span><span class="sxs-lookup"><span data-stu-id="b2fb4-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="b2fb4-106">Microsoft Intune에서 iOS 및 iPadOS 장치에 VPN 설정 추가</span><span class="sxs-lookup"><span data-stu-id="b2fb4-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="b2fb4-107">Intune에서 VPN을 구성하기 위해 Android 장치 설정</span><span class="sxs-lookup"><span data-stu-id="b2fb4-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="b2fb4-108">Microsoft Intune에서 macOS 장치에 VPN 설정 추가</span><span class="sxs-lookup"><span data-stu-id="b2fb4-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="b2fb4-109">VPN 프로필에서 인증서 기반 인증을 사용하는 경우 VPN 프로필에 연결 된 루트 인증서와 클라이언트 인증서 프로필이 성공적으로 배포 되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b2fb4-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="b2fb4-110">**일반적인 문제**</span><span class="sxs-lookup"><span data-stu-id="b2fb4-110">**Common Issues**</span></span>

<span data-ttu-id="b2fb4-111">**장치에 VPN 프로필을 배포 했습니다. Intune에서 성공적으로 연결 되었다고 표시되지만 장치가 VPN에 연결되지 않습니다.**</span><span class="sxs-lookup"><span data-stu-id="b2fb4-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="b2fb4-112">성공 상태는 Intune에서 구성 된 대로 프로필을 배포 했다는 것을 의미합니다.</span><span class="sxs-lookup"><span data-stu-id="b2fb4-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="b2fb4-113">그러나 네트워크 및/또는 인증 요구 사항에 이러한 구성이 맞지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b2fb4-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="b2fb4-114">연결 시도에 대한 자세한 내용은 VPN 서버와 NPS/Radius 서버에 있는 인프라 및 인증 서비스 로그를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b2fb4-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="b2fb4-115">네트워크 인프라 팀 또는 타사 VPN 공급 업체와 협력하여 로그를 수집하고 검토 해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b2fb4-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="b2fb4-116">**iOS용사용자 지정 VPN을 구성할 때 앱별 VPN 기능을 사용할 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="b2fb4-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="b2fb4-117">Intune에서 iOS용 앱별 VPN은 현재 앱별 VPN 구성 전에 인증서 필수 구성 요소를 충족해야 하는 특정 공급자 및 파트너에게만 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="b2fb4-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="b2fb4-118">자세한 내용은 [Intune에서 iOS/iPadOS 장치의 앱별 VPN 설정](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b2fb4-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="b2fb4-119">Intune의 모든 VPN 연결 유형에 대한 자세한 내용은 [Intune에서 VPN 서버 연결을 위한 VPN 프로필 만들기](https://docs.microsoft.com/intune/vpn-settings-configure)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b2fb4-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="b2fb4-120">**구성 된 도메인에 액세스하는 경우 iOS 온-디맨드 VPN이 트리거하지 않음**</span><span class="sxs-lookup"><span data-stu-id="b2fb4-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="b2fb4-121">자동 VPN 설정을 테스트 하려면 다음 값을 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="b2fb4-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="b2fb4-122">다음을 수행하고 싶습니다: **각 연결 시도 평가**</span><span class="sxs-lookup"><span data-stu-id="b2fb4-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="b2fb4-123">연결할 것인지 선택합니다: **필요한 경우 연결**</span><span class="sxs-lookup"><span data-stu-id="b2fb4-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="b2fb4-124">사용자가 이러한 도메인에 액세스 하는 경우: **대상**\* 도메인 이름\*</span><span class="sxs-lookup"><span data-stu-id="b2fb4-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="b2fb4-125">위의 구성이 실패할 경우 다음 요소를 추가 합니다:</span><span class="sxs-lookup"><span data-stu-id="b2fb4-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="b2fb4-126">이 URL에 연결할 수 없는 경우 강제로 VPN에 연결: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="b2fb4-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>