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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733855"
---
# <a name="11-call-recording"></a><span data-ttu-id="693b8-102">1:1 통화 기록</span><span class="sxs-lookup"><span data-stu-id="693b8-102">1:1 call recording</span></span>

<span data-ttu-id="693b8-103">사용자가 1:1 통화를 녹음/녹화할 수 있도록 관리자가 지금 조치를 취해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="693b8-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="693b8-104">2021년 4월 12일부터 새 Teams 통화 정책 옵션 *AllowCloudRecordingForCalls* 적용을 시작할 것입니다.</span><span class="sxs-lookup"><span data-stu-id="693b8-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="693b8-105">현재 1:1 통화 기록 기능은 Teams 모임 정책의 *AllowCloudRecording* 옵션에 의해 제어됩니다.</span><span class="sxs-lookup"><span data-stu-id="693b8-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="693b8-106">사용자가 Teams 모임을 녹음/녹화할 수 있는 경우 1:1 통화도 기록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="693b8-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="693b8-107">모든 사용자가 1:1 통화를 녹음하지 못하게 차단하려면 조치를 취할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="693b8-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="693b8-108">*AllowCloudRecordingForCalls* 호출 정책 옵션은 기본적으로 $False 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="693b8-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="693b8-109">이 변경은 다음 메시지 센터 게시물에 설명되어 있습니다. [(업데이트) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) 통화 기록 정책 소개 Teams 통화 정책 옵션을 설정하려면 Teams PowerShell 을 [사용해야 합니다.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="693b8-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="693b8-110">**1:1** 통화에서 통화 기록을 사용하도록 설정하려면 Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="693b8-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="693b8-111">**1:1** 통화에서 통화 기록을 사용하지 않도록 설정하는 경우: Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="693b8-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

