---
title: 예약된 업데이트를 일시 중지하고 있습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/30/2020
ms.locfileid: "46530591"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="f5c51-102">예약된 업데이트를 일시 중지하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f5c51-102">Pausing scheduled updates</span></span>

<span data-ttu-id="f5c51-103">일시 중지 명령이 실행되면 장치는 다음에 Intune에 체크인할 때까지 명령을 처리하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="f5c51-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="f5c51-104">이 때문에 장치의 구성 요소는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="f5c51-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="f5c51-105">체크인하기 전에 예약된 업데이트를 설치했습니다.</span><span class="sxs-lookup"><span data-stu-id="f5c51-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="f5c51-106">일시 중지 명령을 실행할 때 전원이 꺼졌습니다.</span><span class="sxs-lookup"><span data-stu-id="f5c51-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="f5c51-107">이 경우 장치의 전원을 켜면 체크인하기 전에 예약된 업데이트를 다운로드하여 설치했을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f5c51-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>