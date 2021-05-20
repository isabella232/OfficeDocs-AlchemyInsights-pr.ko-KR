---
title: 9001220 고급 헌팅 사용자 지정 검색
ms.author: dolmont
author: DulceMontemayor
manager: dansimp
ms.date: 09/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200"
- "9001220"
ms.assetid: ''
ms.openlocfilehash: ea478cfbbbe96065608990770e0453d8f2613981
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543007"
---
# <a name="advanced-hunting-custom-detections"></a><span data-ttu-id="9f64b-102">고급 헌팅 사용자 지정 검색</span><span class="sxs-lookup"><span data-stu-id="9f64b-102">Advanced Hunting Custom detections</span></span>

<span data-ttu-id="9f64b-103">고급 헌팅 쿼리를 기반으로 사용자 지정 검색 규칙을 만들고 관리하는 방법을 배울 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9f64b-103">You can learn how to create and manage custom detections rules based on advanced hunting queries.</span></span> <span data-ttu-id="9f64b-104">사용자 지정 검색을 사용하면 위반 활동 및 잘못 구성된 장치를 포함하여 다양한 이벤트 및 시스템 상태의 사전 모니터링 및 대응을 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9f64b-104">With custom detections, you can proactively monitor for and respond to various events and system states, including suspected breach activity and misconfigured devices.</span></span> <span data-ttu-id="9f64b-105">경고 및 응답 작업을 자동으로 트리거하는 사용자 지정 가능한 검색 규칙을 사용하여 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9f64b-105">You can do so with customizable detection rules that automatically trigger alerts and response actions</span></span>
  
<span data-ttu-id="9f64b-106">사용자 Microsoft Defender ATP 자세한 내용은 다음 항목을 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="9f64b-106">If you are using Microsoft Defender ATP, see the following topics for details:</span></span> 
- [<span data-ttu-id="9f64b-107">사용자 지정 검색 개요</span><span class="sxs-lookup"><span data-stu-id="9f64b-107">Custom detections overview</span></span>](/windows/security/threat-protection/microsoft-defender-atp/overview-custom-detections)
- [<span data-ttu-id="9f64b-108">사용자 지정 검색 규칙 만들기</span><span class="sxs-lookup"><span data-stu-id="9f64b-108">Create custom detection rules</span></span>](/windows/security/threat-protection/microsoft-defender-atp/custom-detection-rules)
- [<span data-ttu-id="9f64b-109">사용자 지정 검색 규칙 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="9f64b-109">View and manage custom detection rules</span></span>](/windows/security/threat-protection/microsoft-defender-atp/custom-detections-manage)

<span data-ttu-id="9f64b-110">Defender를 Microsoft 365 자세한 내용은 다음 항목을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9f64b-110">If you are using Microsoft 365 Defender, see the following topics for details:</span></span> 
- [<span data-ttu-id="9f64b-111">사용자 지정 검색 개요</span><span class="sxs-lookup"><span data-stu-id="9f64b-111">Custom detections overview</span></span>](/microsoft-365/security/mtp/custom-detections-overview)
- [<span data-ttu-id="9f64b-112">사용자 지정 검색 규칙 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="9f64b-112">Create and manage custom detections rules</span></span>](/microsoft-365/security/mtp/custom-detection-rules)
