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
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658884"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="1ef02-102">Microsoft Intune에서 Windows 장치 등록 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1ef02-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="1ef02-103">아래에 나열 된 리소스를 검토 하 여 지금 문제를 해결 하세요.</span><span class="sxs-lookup"><span data-stu-id="1ef02-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="1ef02-104">몇 가지 일반적인 오류 메시지 및 해결 단계:</span><span class="sxs-lookup"><span data-stu-id="1ef02-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="1ef02-105">**소프트웨어를 설치할 수 없음, 0x80cf4017:** 계정 인증서가 만료 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef02-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="1ef02-106">Intune 관리 콘솔에서 PC 클라이언트 소프트웨어 패키지를 다시 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef02-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="1ef02-107">자세한 내용은이 설명서를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="1ef02-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="1ef02-108">**오류 코드 0x801c0003:** 이 오류는 다음과 같은 경우에 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef02-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="1ef02-109">사용자에 게 장치 제한 보다 많은 디바이스가 등록 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef02-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="1ef02-110">이러한 문서를 검토 하 여 [장치를 제거](https://docs.microsoft.com/intune/devices-wipe) 하거나 [장치 제한을 변경](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef02-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="1ef02-111">"사용자가 Azure AD에 장치를 연결할 수 있습니다."가 "없음"으로 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ef02-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="1ef02-112">모두로 설정 하거나 사용자를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef02-112">Set it to all or select users.</span></span> <span data-ttu-id="1ef02-113">자세한 내용은 [이 설명서](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) 를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="1ef02-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="1ef02-114">다른 사용자가 장치를 이미 등록 했습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef02-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="1ef02-115">이 경우에는 다시 시도 하기 전에 Azure Intune 콘솔에서 장치를 제거 하거나 장치를 수동으로 등록 취소 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef02-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="1ef02-116">장치가 Windows 10 Home입니다.</span><span class="sxs-lookup"><span data-stu-id="1ef02-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="1ef02-117">Windows 10 Pro, 교육 및 Enterprise Sku만 Azure Active Directory에 참가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef02-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="1ef02-118">문제를 해결 하는 데 도움이 되는 추가 리소스:</span><span class="sxs-lookup"><span data-stu-id="1ef02-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="1ef02-119">[Intune 문제 해결 포털](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 을 사용 하 여 일반적인 등록 오류를 진단 하 고 해결 합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef02-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="1ef02-120">자세한 내용을 보려면 [이 문서](https://docs.microsoft.com/intune/help-desk-operators) 를 검토 하세요.</span><span class="sxs-lookup"><span data-stu-id="1ef02-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="1ef02-121">다음 문서를 검토하여 등록과 해결 방법을 방지하는 일반적인 오류의 목록을 확인합니다. [문제 해결 가이드](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) 및 [문제 해결 문서](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="1ef02-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="1ef02-122">[Microsoft Intune에서 Windows 장치를 등록 하는 방법에 대해 알아봅니다](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="1ef02-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
