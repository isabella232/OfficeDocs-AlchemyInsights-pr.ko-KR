---
title: Microsoft Edge에서 개인 정보 설정 구성
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403859"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="17cab-102">Microsoft Edge에서 개인 정보 설정 구성</span><span class="sxs-lookup"><span data-stu-id="17cab-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="17cab-103">기본적으로 Microsoft Edge가 비 Windows 플랫폼에 배포되어 있는 경우 진단 데이터 및 사이트 정보는 Microsoft로 전송되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="17cab-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="17cab-104">그러나 Microsoft Edge가 Windows 10에 배포된 경우 진단 데이터 및 사이트 정보는 사용자의 Windows 진단 데이터 설정 [에 따라 전송됩니다.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="17cab-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="17cab-105">Microsoft Edge에서 조직의 데이터 수집을 처리하는 방법을 구성하기 위해 다음 그룹 정책을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="17cab-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="17cab-106">[MetricsReportingEnabled는](https://go.microsoft.com/fwlink/?linkid=2132470) 사용 현황 및 크래시 관련 데이터에 대한 보고를 하게 합니다.</span><span class="sxs-lookup"><span data-stu-id="17cab-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="17cab-107">[SendSiteInfoToImproveServices는](https://go.microsoft.com/fwlink/?linkid=2132470) Microsoft 서비스를 개선하는 데 사용되는 사이트 정보를 전송합니다.</span><span class="sxs-lookup"><span data-stu-id="17cab-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="17cab-108">자세한 내용은 정책 설정 [구성을 참조하세요.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="17cab-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
