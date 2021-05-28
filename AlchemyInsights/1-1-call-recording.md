---
title: 1:1 통화 기록
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696964"
---
# <a name="11-call-recording"></a><span data-ttu-id="8d7b9-102">1:1 통화 기록</span><span class="sxs-lookup"><span data-stu-id="8d7b9-102">1:1 call recording</span></span>

<span data-ttu-id="8d7b9-103">녹음 **시작 단추가** 1:1 통화에서 회색으로 표시되어 있는 경우 영향을 미치는 사용자에 대한 정책 설정을 변경해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8d7b9-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="8d7b9-104">2021년 5월 31일부터 새 통화 정책 *AllowCloudRecordingForCalls* Teams 적용을 시작할 것입니다.</span><span class="sxs-lookup"><span data-stu-id="8d7b9-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="8d7b9-105">이 변경 이전에는 1:1 통화 기록이 *AllowCloudRecording* 및 모임 정책에 Teams 제어됩니다.</span><span class="sxs-lookup"><span data-stu-id="8d7b9-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="8d7b9-106">이 변경은 메시지 센터 게시물: [(업데이트) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)통화 기록 정책 소개에 설명되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8d7b9-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="8d7b9-107">*AllowCloudRecordingForCalls*   통화 정책 옵션은 기본적으로 $False **설정되어** 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8d7b9-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="8d7b9-108">모든 사용자가 1:1 통화를 녹음하지 못하게 차단하려면 조치를 취할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8d7b9-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="8d7b9-109">1:1 통화의 모든 사용자에 대해 통화 기록을 사용하도록 설정하려면 powerShell에서 Teams cmdlet을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="8d7b9-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="8d7b9-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="8d7b9-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="8d7b9-111">또는 새 정책을 만들고 **-AllowCloudRecordingForCalls를** $true  정책을 사용자에게 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8d7b9-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="8d7b9-112">자세한 내용은 1:1 통화 기록 정책 [컨트롤은 거의(거의!)를 참조하세요. 여기에서 을(를)](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)클릭</span><span class="sxs-lookup"><span data-stu-id="8d7b9-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
