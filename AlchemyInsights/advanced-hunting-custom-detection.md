---
title: 9001220 고급 구하기 사용자 지정 검색
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
ms.openlocfilehash: 40351bd7852b69e0ff2ae6f630749ecbc1e0f13b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801521"
---
# <a name="advanced-hunting-custom-detections"></a><span data-ttu-id="8d633-102">고급 구하기 사용자 지정 검색</span><span class="sxs-lookup"><span data-stu-id="8d633-102">Advanced Hunting Custom detections</span></span>

<span data-ttu-id="8d633-103">고급 검색 쿼리를 기반으로 사용자 지정 검색 규칙을 만들고 관리 하는 방법에 대해 알아볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8d633-103">You can learn how to create and manage custom detections rules based on advanced hunting queries.</span></span> <span data-ttu-id="8d633-104">사용자 지정 검색을 사용 하면 의심 스러운 위반 작업과 잘못 구성 된 장치를 포함 하 여 다양 한 이벤트 및 시스템 상태를 사전에 모니터링 하 고 응답할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8d633-104">With custom detections, you can proactively monitor for and respond to various events and system states, including suspected breach activity and misconfigured devices.</span></span> <span data-ttu-id="8d633-105">이렇게 하려면 경고 및 응답 작업을 자동으로 트리거하는 사용자 지정 가능한 검색 규칙을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8d633-105">You can do so with customizable detection rules that automatically trigger alerts and response actions</span></span>
  
<span data-ttu-id="8d633-106">Microsoft Defender ATP를 사용 하는 경우 자세한 내용은 다음 항목을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="8d633-106">If you are using Microsoft Defender ATP, see the following topics for details:</span></span> 
- [<span data-ttu-id="8d633-107">사용자 지정 검색 개요</span><span class="sxs-lookup"><span data-stu-id="8d633-107">Custom detections overview</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/overview-custom-detections)
- [<span data-ttu-id="8d633-108">사용자 지정 검색 규칙 만들기</span><span class="sxs-lookup"><span data-stu-id="8d633-108">Create custom detection rules</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/custom-detection-rules)
- [<span data-ttu-id="8d633-109">사용자 지정 검색 규칙 보기 및 관리</span><span class="sxs-lookup"><span data-stu-id="8d633-109">View and manage custom detection rules</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/custom-detections-manage)

<span data-ttu-id="8d633-110">Microsoft 365 Defender를 사용 하는 경우 자세한 내용은 다음 항목을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="8d633-110">If you are using Microsoft 365 Defender, see the following topics for details:</span></span> 
- [<span data-ttu-id="8d633-111">사용자 지정 검색 개요</span><span class="sxs-lookup"><span data-stu-id="8d633-111">Custom detections overview</span></span>](https://docs.microsoft.com/microsoft-365/security/mtp/custom-detections-overview)
- [<span data-ttu-id="8d633-112">사용자 지정 검색 규칙 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="8d633-112">Create and manage custom detections rules</span></span>](https://docs.microsoft.com/microsoft-365/security/mtp/custom-detection-rules)
