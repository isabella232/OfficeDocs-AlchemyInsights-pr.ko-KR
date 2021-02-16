---
title: 디바이스 사용
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
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255180"
---
# <a name="enable-device"></a><span data-ttu-id="eacd5-102">디바이스 사용</span><span class="sxs-lookup"><span data-stu-id="eacd5-102">Enable Device</span></span>

<span data-ttu-id="eacd5-103">**Powershell 명령을 사용하여 디바이스를 사용하도록 설정하려면**</span><span class="sxs-lookup"><span data-stu-id="eacd5-103">**To enable the device using Powershell command**</span></span>

<span data-ttu-id="eacd5-104">다음의 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="eacd5-104">Run the following commands:</span></span>

- <span data-ttu-id="eacd5-105">장치 개체를 얻하려면 `Get-MsolDevice -Name <Name>`</span><span class="sxs-lookup"><span data-stu-id="eacd5-105">To get device object: `Get-MsolDevice -Name <Name>`</span></span>
- <span data-ttu-id="eacd5-106">디바이스를 사용하도록 설정하려면 `Enable-MsolDevice -DeviceId <DeviceId>`</span><span class="sxs-lookup"><span data-stu-id="eacd5-106">To enable device: `Enable-MsolDevice -DeviceId <DeviceId>`</span></span>

<span data-ttu-id="eacd5-107">관리되는 도메인에서 하이브리드 가입 구성에 대한 자세한 내용은 하이브리드 가입 [구성을 참조하세요.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)</span><span class="sxs-lookup"><span data-stu-id="eacd5-107">For more information on Configuring Hybrid Join on managed domains, see [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span></span>
