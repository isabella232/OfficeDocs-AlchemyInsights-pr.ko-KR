---
title: Intune Wi-Fi 프로필
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
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696267"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="43d99-102">Intune Wi-Fi 프로필</span><span class="sxs-lookup"><span data-stu-id="43d99-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="43d99-103">MDM 클라이언트용 Wi-Fi 연결의 성공적인 구현은 회사 Wi-Fi 인프라의 요구 사항을 반영하는 올바르게 배포된 프로필에 따라 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="43d99-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="43d99-104">조사 중인 클라이언트 플랫폼의 적절한 설정을 검토하려면 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="43d99-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="43d99-105">Microsoft Intune에서 Android를 실행하는 장치의 Wi-Fi 설정 추가</span><span class="sxs-lookup"><span data-stu-id="43d99-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="43d99-106">Android Enterprise 전용 Wi-Fi 설정 및 Microsoft Intune에서 완전히 관리되는 장치 추가</span><span class="sxs-lookup"><span data-stu-id="43d99-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="43d99-107">Microsoft Intune에서 iOS 및 iPadOS 장치용 Wi-Fi 설정 추가</span><span class="sxs-lookup"><span data-stu-id="43d99-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="43d99-108">Intune에서 Windows 10 이상 장치용 Wi-Fi 설정 추가</span><span class="sxs-lookup"><span data-stu-id="43d99-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="43d99-109">Intune에서 Windows 장치용 Wi-Fi 설정 추가</span><span class="sxs-lookup"><span data-stu-id="43d99-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="43d99-110">**일반적인 문제**</span><span class="sxs-lookup"><span data-stu-id="43d99-110">**Common Issues**</span></span>

<span data-ttu-id="43d99-111">**Wi-Fi 프로필에 지정된 배포 인증서에 종속된 Wi-Fi 프로필을 배포하는 중입니다. 그러나 구성 프로필에 오류 상태가 표시됩니다.**</span><span class="sxs-lookup"><span data-stu-id="43d99-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="43d99-112">장치에 인증서를 받았는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="43d99-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="43d99-113">Intune에서 **모든 장치**로 이동하여 장치 > **장치 구성**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="43d99-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="43d99-114">모든 예상 프로필이 성공적인 상태로 나열되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="43d99-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="43d99-115">Android 프로필의 경우 인증서 체인에 중간 인증서가 있는 경우 해당 인증서가 Android 장치에 배포되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="43d99-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="43d99-116">인증서 상태를 확인하려면 **장치 구성** > **프로필** > **Android 중간 CA** > **속성** > **신뢰하는 인증서**로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="43d99-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="43d99-117">오류가 계속 발생하는 경우 절차와 문제 해결 섹션을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="43d99-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="43d99-118">자세한 내용은 [Microsoft Intune에서 SCEP 인증서 프로필 문제 해결에 대한 개요](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="43d99-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="43d99-119">**장치에 Wi-Fi 프로필을 배포했습니다. Intune에서 성공적으로 연결되었다고 표시되지만 장치가 Wi-Fi에 연결되지 않습니다.**</span><span class="sxs-lookup"><span data-stu-id="43d99-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="43d99-120">성공 상태는 Intune에서 구성 된 대로 프로필을 배포 했다는 것을 의미합니다.</span><span class="sxs-lookup"><span data-stu-id="43d99-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="43d99-121">그러나 네트워크 및/또는 인증 요구 사항에 이러한 구성이 맞지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43d99-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="43d99-122">연결 시도에 대한 자세한 내용은 (Wi-Fi 액세스 포인트 컨트롤러 및 NPS/Radium 서버에 있는) 인프라 및 인증 서비스 내 로그를 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="43d99-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="43d99-123">네트워크 인프라 팀 또는 타사 Wi-Fi 공급 업체와 협력하여 로그를 수집하고 검토해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43d99-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>