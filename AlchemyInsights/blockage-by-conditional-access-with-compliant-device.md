---
title: 규격 장치를 사용하여 조건부 액세스에서 차단되는 경우
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897982"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a><span data-ttu-id="a28b3-102">규격 장치를 사용하여 조건부 액세스에서 차단되는 경우</span><span class="sxs-lookup"><span data-stu-id="a28b3-102">I’m getting blocked by Conditional Access with compliant device</span></span>

<span data-ttu-id="a28b3-103">**권장 도구**</span><span class="sxs-lookup"><span data-stu-id="a28b3-103">**Highly Recommended Tools**</span></span>

- <span data-ttu-id="a28b3-104">[장치 등록 문제 도구](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - 가장 일반적인 장치 등록 문제를 해결하는 데 도움이 되는 포괄적인 도구입니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - A comprehensive tool that helps troubleshoot the most common device registration issues.</span></span>
- <span data-ttu-id="a28b3-105">[장치 등록 연결 스크립트 테스트](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - 장치가 시스템 계정 아래에 있는 장치 등록 끝점에 액세스할 수 있는지를 확인하는 데 사용되는 도구입니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - A tool used to ensure that a device can access Device Registration endpoints under the system account.</span></span>
- <span data-ttu-id="a28b3-106">[Azure AD 장치 정리 스크립트](https://github.com/mzmaili/AzureADDeviceCleanup) - 환경에서 오래된 장치를 검색하고 관리하는 데 사용되는 도구입니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - A tool used to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="a28b3-107">다음은 규격 장치에 대한 조건부 액세스가 실패하는 일반적인 이유 또는 조직 리소스에 대한 로그인 요청 중에 사용자가 **여기서는 연결할 수 없습니다** 메시지를 수신하는 몇 가지 일반적인 이유입니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-107">Here are some common reasons why Conditional Access may be failing for a compliant device or why your users may be receiving **You can't get there from here** message during a sign-in request to an organizational resource.</span></span>

1. <span data-ttu-id="a28b3-108">**장치가 MDM과 함께 필요한 장치 상태가 아닌 경우**:</span><span class="sxs-lookup"><span data-stu-id="a28b3-108">**Device is not in a required device state with an MDM**:</span></span>

<span data-ttu-id="a28b3-109">장치가 Intune과 같은 승인된 MDM 제공자에 등록되어 있고 *준수* 로 표시되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-109">Validate that the device is enrolled with an approved MDM provider like Intune and *marked as compliant*.</span></span> <span data-ttu-id="a28b3-110">Intune에 대한 Intune자세한 내용은 이 [문서](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="a28b3-110">For more information on Intune see this [document](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment).</span></span> <span data-ttu-id="a28b3-111">장치 규정 준수 및 Intune에 대한 자세한 내용은 [규정 준수 정책을 사용하여 Intune으로 관리하는 장치에 대한 규칙을 설정](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a28b3-111">For better understanding of device compliance and Intune, see [use compliance policy to set rules for devices you manage with Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started).</span></span> <span data-ttu-id="a28b3-112">장치를 Intune으로 등록하는 데 문제가 있는 경우 [Microsoft의 장치 등록 문제 해결](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)에서 문제 해결 세부 정보를 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-112">If you are having issues enrolling a device with Intune, find troubleshooting details at [Troubleshoot device enrollment in Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span> <span data-ttu-id="a28b3-113">Intune 지원에 대한 지원 요청은 지원 요청을 작성하세요.</span><span class="sxs-lookup"><span data-stu-id="a28b3-113">For further Intune support, create a support request.</span></span> <span data-ttu-id="a28b3-114">지원 요청을 작성하려면 [Intune 도움말 및 지원 페이지](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)를 방문하세요.</span><span class="sxs-lookup"><span data-stu-id="a28b3-114">To do so, visit the [Intune Help and Support page](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).</span></span>

2. <span data-ttu-id="a28b3-115">**장치가 조직 네트워크에 연결되어 있지 않은 경우**:</span><span class="sxs-lookup"><span data-stu-id="a28b3-115">**Device is not joined to the organizations network**:</span></span>

<span data-ttu-id="a28b3-116">조직 리소스에 액세스하려면 장치를 직접 연결 또는 VPN(가상 사설망)을 통해 조직의 네트워크에 연결하고 온-프레미스 또는 Azure Active Directory에도 연결해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-116">For access to organizational resources, the device has to be connected to the organization's network, either through direct connection or a virtual private network (VPN), and also joined to on-premise or Azure Active Directory.</span></span> <span data-ttu-id="a28b3-117">조직 장치를 조직 네트워크에 연결하려면 [조직 장치를 조직 네트워크에 연결](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a28b3-117">To join a work device to the organization network, see [Join your work device to your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network).</span></span> <span data-ttu-id="a28b3-118">개인/BYOD 장치를 등록하려면 [개인 장치를 조직 네트워크에 연결](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a28b3-118">To register a personal/BYOD device, see [Register your personal device on your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).</span></span>

- <span data-ttu-id="a28b3-119">장치가 네트워크에 연결되어 있는지 확인하려면 단계에 따라 [여기](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered)에서 등록된 장치를 확인하거나 [여기](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined)에서 작동 중인 장치를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="a28b3-119">To validate whether the device has joined the network, you can follow the steps for registered devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) or work devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined).</span></span> <span data-ttu-id="a28b3-120">조직 네트워크 연결 문제를 범위 지정하려면 다음 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="a28b3-120">To scope the issue to Org network connectivity, follow guidelines below:</span></span>

    1. <span data-ttu-id="a28b3-121">회사 또는 학교 계정(예: alain@contoso.com)을 사용하여 Windows에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-121">Sign in to Windows using your work or school account,  for example, alain@contoso.com.</span></span>
    2. <span data-ttu-id="a28b3-122">VPN이나 DirectAccess를 통해 조직 네트워크에 연결합니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-122">Connect to your organization's network through a VPN or DirectAccess.</span></span>
    3. <span data-ttu-id="a28b3-123">연결한 후, **Windows 로고 키 + L** 을 눌러 장치를 잠급니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-123">After you're connected, press the **Windows logo key+L** to lock your device.</span></span>
    4. <span data-ttu-id="a28b3-124">회사 또는 학교 계정을 사용하여 장치를 잠금 해제하고 문제가 있는 앱이나 서비스에 다시 액세스합니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-124">Unlock your device using your work or school account, and then try to access the problematic app or service again.</span></span>

<span data-ttu-id="a28b3-125">**여기서는 불가능합니다** 오류 메시지가 다시 표시되면, 다른 곳에서 문제가 발생할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-125">If you see the **You can't get there from here** error message again, issue is likely elsewhere.</span></span>

3. <span data-ttu-id="a28b3-126">**운영 체제가 지원되지 않는 경우**:</span><span class="sxs-lookup"><span data-stu-id="a28b3-126">**Operating system is not supported**:</span></span>

<span data-ttu-id="a28b3-127">다음을 포함한 지원되는 버전에서 실행 중인지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-127">Ensure that you're running a supported version of the operating system, including:</span></span>

- <span data-ttu-id="a28b3-128">**Windows 클라이언트**: Windows 7 또는 이상</span><span class="sxs-lookup"><span data-stu-id="a28b3-128">**Windows Client**: Windows 7 or later</span></span>

- <span data-ttu-id="a28b3-129">**Windows Server**: Windows Server 2008 R2 또는 이상</span><span class="sxs-lookup"><span data-stu-id="a28b3-129">**Windows Server**: Windows Server 2008 R2 or later</span></span>

- <span data-ttu-id="a28b3-130">**macOS**: macOS X 또는 이상</span><span class="sxs-lookup"><span data-stu-id="a28b3-130">**macOS**: macOS X or later</span></span>

- <span data-ttu-id="a28b3-131">**Android 및 iOS**: 최신 버전의 Android 및 iOS 모바일 운영 체제</span><span class="sxs-lookup"><span data-stu-id="a28b3-131">**Android and iOS**: Latest version of Android and iOS mobile operating systems</span></span>

4. <span data-ttu-id="a28b3-132">**지원되지 않는 웹 브라우저의 경우**:</span><span class="sxs-lookup"><span data-stu-id="a28b3-132">**Web browser is not supported**:</span></span>

<span data-ttu-id="a28b3-133">아래에서 지원되는 브라우저를 찾아 보세요.</span><span class="sxs-lookup"><span data-stu-id="a28b3-133">Please find supported browsers below.</span></span> <span data-ttu-id="a28b3-134">Windows 1703 이상 버전에서 Chrome을 지원하려면 Windows 10 계정 확장이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-134">For Chrome support with Windows 1703 or later versions, a Windows 10 Accounts extension is required.</span></span> <span data-ttu-id="a28b3-135">Edge 85 이상의 경우 장치 규정 준수 정보를 제대로 전달하려면 사용자가 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a28b3-135">For Edge 85+, the user needs to be signed in to properly pass device compliance information.</span></span> <span data-ttu-id="a28b3-136">자세한 내용은 [여기](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a28b3-136">For more details, see [here](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

- <span data-ttu-id="a28b3-137">**Windows 10**: Microsoft Edge, Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="a28b3-137">**Windows 10**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="a28b3-138">**Windows 8/8.1**: Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="a28b3-138">**Windows 8 / 8.1**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="a28b3-139">**Windows 7**: Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="a28b3-139">**Windows 7**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="a28b3-140">**iOS**: Microsoft Edge, Intune 관리되는 브라우저, Safari</span><span class="sxs-lookup"><span data-stu-id="a28b3-140">**iOS**: Microsoft Edge, Intune Managed Browser, Safari</span></span>
- <span data-ttu-id="a28b3-141">**Android**: **Microsoft Edge**: Intune 관리되는 브라우저, Chrome</span><span class="sxs-lookup"><span data-stu-id="a28b3-141">**Android**: **Microsoft Edge**: Intune Managed Browser, Chrome</span></span>
- <span data-ttu-id="a28b3-142">**Windows 휴대폰**: Microsoft Edge, Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="a28b3-142">**Windows Phone**: Microsoft Edge, Internet Explorer</span></span>
- <span data-ttu-id="a28b3-143">**Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome</span><span class="sxs-lookup"><span data-stu-id="a28b3-143">**Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="a28b3-144">**Windows Server 2016**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="a28b3-144">**Windows Server 2016**: Internet Explorer</span></span>
- <span data-ttu-id="a28b3-145">**Windows Server 2012 R2**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="a28b3-145">**Windows Server 2012 R2**: Internet Explorer</span></span>
- <span data-ttu-id="a28b3-146">**Windows Server 2008 R2**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="a28b3-146">**Windows Server 2008 R2**: Internet Explorer</span></span>
- <span data-ttu-id="a28b3-147">**macOS**: Chrome, Safari</span><span class="sxs-lookup"><span data-stu-id="a28b3-147">**macOS**: Chrome, Safari</span></span>

<span data-ttu-id="a28b3-148">**여기에서는 불가능합니다** 에 대한 자세한 내용은 메시지와 [여기](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)의 문제 해결 단계를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a28b3-148">Find more information on the **You can't get there** message and troubleshooting steps [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).</span></span>
