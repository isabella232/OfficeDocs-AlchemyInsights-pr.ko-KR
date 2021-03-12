---
title: Microsoft Intune에서 Windows 장치 등록 문제 해결
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708896"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="d064e-102">Microsoft Intune에서 Windows 장치 등록 문제 해결</span><span class="sxs-lookup"><span data-stu-id="d064e-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="d064e-103">아래 나열된 리소스를 검토하여 지금 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="d064e-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d064e-104">몇 가지 일반적인 오류 메시지 및 해결 단계:</span><span class="sxs-lookup"><span data-stu-id="d064e-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="d064e-105">**다음을 위해 소프트웨어를** 설치할 0x80cf4017. 계정 인증서가 만료되었습니다.</span><span class="sxs-lookup"><span data-stu-id="d064e-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="d064e-106">Intune 관리 콘솔에서 PC 클라이언트 소프트웨어 패키지를 다시 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="d064e-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="d064e-107">자세한 내용은 이 설명서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d064e-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="d064e-108">**오류 코드 0x801c0003:** 이 오류는 다음과 같은 시나리오에서 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d064e-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="d064e-109">사용자가 장치 제한보다 더 많은 장치를 등록했습니다.</span><span class="sxs-lookup"><span data-stu-id="d064e-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="d064e-110">이러한 문서를 검토하여 장치를 [제거하거나](https://docs.microsoft.com/intune/devices-wipe) 장치 [제한을 변경합니다.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="d064e-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="d064e-111">"사용자가 장치를 Azure AD에 가입할 수 있습니다."는 "없음"으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="d064e-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="d064e-112">전체로 설정하거나 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="d064e-112">Set it to all or select users.</span></span> <span data-ttu-id="d064e-113">자세한 [내용은 이](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) 설명서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d064e-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="d064e-114">디바이스가 이미 다른 사용자가 등록했습니다.</span><span class="sxs-lookup"><span data-stu-id="d064e-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="d064e-115">이 경우 다시 시도하기 전에 Azure Intune 콘솔에서 장치를 제거하거나 수동으로 디바이스의 구독을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="d064e-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="d064e-116">디바이스가 Windows 10 Home입니다.</span><span class="sxs-lookup"><span data-stu-id="d064e-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="d064e-117">Windows 10 Pro, Education 및 Enterprise SKUS만 Azure Active Directory에 가입할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d064e-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="d064e-118">문제를 해결하는 데 도움이 되는 추가 리소스:</span><span class="sxs-lookup"><span data-stu-id="d064e-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="d064e-119">[Intune 문제 해결 포털을](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 사용하여 일반적인 등록 실패를 진단하고 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="d064e-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d064e-120">자세한 [내용은 이](https://docs.microsoft.com/intune/help-desk-operators) 문서를 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="d064e-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="d064e-121">다음 문서를 검토하여 등록과 해결 방법을 방지하는 일반적인 오류의 목록을 확인합니다. [문제 해결 가이드](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) 및 [문제 해결 문서](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="d064e-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="d064e-122">[Microsoft Intune에서 Windows 장치를 등록하는 방법을 학습합니다.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="d064e-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
