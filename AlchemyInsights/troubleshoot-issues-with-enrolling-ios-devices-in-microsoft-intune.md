---
title: Microsoft Intune에서 iOS 장치 등록 시 발생 하는 문제 해결
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669254"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="e8f07-102">Microsoft Intune에서 iOS 장치 등록 시 발생 하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e8f07-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="e8f07-103">아래에 나열 된 리소스를 검토 하 여 지금 문제를 해결 하세요.</span><span class="sxs-lookup"><span data-stu-id="e8f07-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="e8f07-104">몇 가지 일반적인 오류 메시지 및 해결 단계:</span><span class="sxs-lookup"><span data-stu-id="e8f07-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="e8f07-105">**장치 Cap에 도달 함** 사용자에 게 장치 제한 보다 많은 디바이스가 등록 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e8f07-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="e8f07-106">이러한 문서를 검토 하 여 [장치를 제거](https://docs.microsoft.com/intune/devices-wipe) 하거나 [장치 제한을 변경](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)합니다.</span><span class="sxs-lookup"><span data-stu-id="e8f07-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="e8f07-107">**이 서비스는 지원 되지 않습니다. 등록 정책 없음:** APNS (Apple Push Notification Service)를 구성 하거나 갱신 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e8f07-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="e8f07-108">이 작업을 수행 하는 방법에 대 한 지침은 [이 문서](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) 를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="e8f07-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="e8f07-109">**사용자 라이선스 유형이 잘못 되었거나 사용자 이름을 인식할 수 없습니다.** 사용자에 게 Intune 또는 EMS 라이선스를 할당 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e8f07-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="e8f07-110">[Office 관리 센터](https://docs.microsoft.com/intune/licenses-assign) 또는 [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups)을 통해 라이선스를 할당 하려면 다음 문서를 검토 하세요.</span><span class="sxs-lookup"><span data-stu-id="e8f07-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="e8f07-111">문제를 해결 하는 데 도움이 되는 추가 리소스:</span><span class="sxs-lookup"><span data-stu-id="e8f07-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e8f07-112">[Intune 문제 해결 포털](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 을 사용 하 여 일반적인 등록 오류를 진단 하 고 해결 합니다.</span><span class="sxs-lookup"><span data-stu-id="e8f07-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e8f07-113">자세한 내용을 보려면 [이 문서](https://docs.microsoft.com/intune/help-desk-operators) 를 검토 하세요.</span><span class="sxs-lookup"><span data-stu-id="e8f07-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="e8f07-114">다음 문서를 검토하여 등록과 해결 방법을 방지하는 일반적인 오류의 목록을 확인합니다. [문제 해결 가이드](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) 및 [문제 해결 문서](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e8f07-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="e8f07-115">[Microsoft Intune에서 iOS 장치를 등록 하는 방법을 알아봅니다](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="e8f07-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

