---
title: Microsoft Intune에서 DEP 등록 문제 해결
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: f76e47c2a3007175ae1bfbd9d20cb59513eb713b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708716"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="1efbe-102">Microsoft Intune에서 DEP 등록 문제 해결</span><span class="sxs-lookup"><span data-stu-id="1efbe-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="1efbe-103">아래 나열된 리소스를 검토하여 지금 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="1efbe-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="1efbe-104">DEP 장치가 등록할 수 없는 경우 MFA(Multi-Factor Authentication)를 사용하도록 설정한 경우 MFA를 사용하지 않도록 설정하세요.</span><span class="sxs-lookup"><span data-stu-id="1efbe-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="1efbe-105">현재 DEP 등록에 대해 MFA가 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1efbe-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="1efbe-106">[Intune 문제 해결 포털을](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 사용하여 일반적인 등록 실패를 진단하고 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="1efbe-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="1efbe-107">자세한 [내용은 이](https://docs.microsoft.com/intune/help-desk-operators) 문서를 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="1efbe-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="1efbe-108">각 문서에 등록 및 해결을 방지하는 일반적인 오류 목록은 문제 해결 [가이드](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) 및 문제 해결 [문서를 참조하세요.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="1efbe-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="1efbe-109">[장치 등록 프로그램에 대해 자세히 알아보시다.](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios)</span><span class="sxs-lookup"><span data-stu-id="1efbe-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>
