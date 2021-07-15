---
title: 화면 공유 품질
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11061"
- "11062"
- "9002254"
- "9002536"
ms.openlocfilehash: 0832f886d3f5c0bfbfe138647403e4e215deaacb
ms.sourcegitcommit: d822377ec76adf9ef6d13bc761a16c9900a3e7cb
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/26/2021
ms.locfileid: "52027306"
---
# <a name="screen-sharing-quality"></a><span data-ttu-id="b6201-102">화면 공유 품질</span><span class="sxs-lookup"><span data-stu-id="b6201-102">Screen sharing quality</span></span>

<span data-ttu-id="b6201-103">대부분의 경우 화면 공유의 품질 문제는 클라이언트 측의 제한된 대역폭으로 인해 발생한 것입니다.</span><span class="sxs-lookup"><span data-stu-id="b6201-103">In most cases quality issues with Screen Sharing comes down to limited bandwidth from the client side.</span></span>  <span data-ttu-id="b6201-104">대역폭이 제한되지 않은 경우, Teams에서는 최대 1080p 비디오 해상도, 비디오의 경우 최대 30fps, 콘텐츠의 경우 15fps, 고음질 오디오를 포함하여 미디어 품질을 최적화합니다.</span><span class="sxs-lookup"><span data-stu-id="b6201-104">Where bandwidth isn't limited, Teams optimizes media quality, including up to 1080p video resolution, up to 30fps for video and 15fps for content, and high-fidelity audio.</span></span>

<span data-ttu-id="b6201-105">Teams는 항상 대역폭 사용에 대해 보수적이며 1.2Mbps 미만에서 HD 비디오 품질을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b6201-105">Teams is always conservative on bandwidth utilization and can deliver HD video quality in under 1.2Mbps.</span></span> <span data-ttu-id="b6201-106">각 오디오/비디오 통화 또는 모임에서 실제 대역폭 소비량은 비디오 레이아웃, 비디오 해상도, 초당 비디오 프레임 등 여러 요인에 따라 달라집니다.</span><span class="sxs-lookup"><span data-stu-id="b6201-106">The actual bandwidth consumption in each audio/video call or meeting vary based on factors such as video layout, video resolution, and video frames per second.</span></span> <span data-ttu-id="b6201-107">대역폭을 더 많이 사용할 수 있게 되면 최상의 환경을 제공하기 위해 품질이 향상되고 사용량이 늘어납니다.</span><span class="sxs-lookup"><span data-stu-id="b6201-107">When more bandwidth is available, quality and usage increase to deliver the best experience.</span></span> <span data-ttu-id="b6201-108">이 표는 Teams에서 대역폭을 사용하는 방법에 대해 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="b6201-108">This table describes how Teams uses bandwidth:</span></span>

<span data-ttu-id="b6201-109">**대역폭(업/다운) 시나리오**</span><span class="sxs-lookup"><span data-stu-id="b6201-109">**Bandwidth(up/down) Scenarios**</span></span>

- <span data-ttu-id="b6201-110">30kbps 피어 투 피어 음성 통화</span><span class="sxs-lookup"><span data-stu-id="b6201-110">30 kbps Peer-to-peer audio calling</span></span>

- <span data-ttu-id="b6201-111">130kbps 피어 투 피어 음성 통화 및 화면 공유</span><span class="sxs-lookup"><span data-stu-id="b6201-111">130 kbps Peer-to-peer audio calling and screen sharing</span></span>

- <span data-ttu-id="b6201-112">30fps에서 500kbps의 피어 투 피어 품질 영상 통화 360p</span><span class="sxs-lookup"><span data-stu-id="b6201-112">500 kbps Peer-to-peer quality video calling 360p at 30fps</span></span>

- <span data-ttu-id="b6201-113">30fps에서 1.2Mbps 피어 투 피어 HD 화질 영상 통화, 해상도 HD 720p</span><span class="sxs-lookup"><span data-stu-id="b6201-113">1.2 Mbps Peer-to-peer HD quality video calling with resolution of HD 720p at 30fps</span></span>

- <span data-ttu-id="b6201-114">30fps에서 1.5Mbps 피어 투 피어 HD 화질 영상 통화, 해상도 HD 1080p</span><span class="sxs-lookup"><span data-stu-id="b6201-114">1.5 Mbps Peer-to-peer HD quality video calling with resolution of HD 1080p at 30fps</span></span>

- <span data-ttu-id="b6201-115">500kbps/1Mbps 그룹 영상 통화</span><span class="sxs-lookup"><span data-stu-id="b6201-115">500kbps/1Mbps Group Video calling</span></span>

- <span data-ttu-id="b6201-116">1Mbps/2Mbps HD 그룹 영상 통화(1080p 화면의 540p 비디오)</span><span class="sxs-lookup"><span data-stu-id="b6201-116">1Mbps/2Mbps HD Group video calling (540p videos on 1080p screen)</span></span>

<span data-ttu-id="b6201-117">자세한 정보는 [Microsoft Teams를 위한 조직 네트워크 준비](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b6201-117">For more information, see [Prepare your organization's network for Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span></span>