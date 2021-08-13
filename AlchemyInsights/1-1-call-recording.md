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
ms.openlocfilehash: befb89c28396be3dc60d9d812a0c6aced69bea3c1c48d88a4ab81a34d6c259b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918997"
---
# <a name="11-call-recording"></a>1:1 통화 기록

녹음 **시작 단추가** 1:1 통화에서 회색으로 표시되어 있는 경우 영향을 미치는 사용자에 대한 정책 설정을 변경해야 합니다. 정책 설정을 확인하기 위해 위의 1:1 통화 기록: 진단: Teams **1:1** 통화 기록을 입력하여 영향을 Teams 진단을 실행합니다.     

2021년 5월 31일부터 새 통화 정책 *AllowCloudRecordingForCalls* Teams 적용을 시작할 것입니다. 이 변경 이전에는 1:1 통화 기록이 *AllowCloudRecording* 및 모임 정책에 Teams 제어됩니다. 이 변경은 메시지 센터 게시물: [(업데이트) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)통화 기록 정책 소개에 설명되어 있습니다.  

*AllowCloudRecordingForCalls*   통화 정책 옵션은 기본적으로 $False **설정되어** 있습니다. 모든 사용자가 1:1 통화를 녹음하지 못하게 차단하려면 조치를 취할 필요가 없습니다.  

1:1 통화의 모든 사용자에 대해 통화 기록을 사용하도록 설정하려면 [powerShell에서](/microsoftteams/teams-powershell-install) Teams cmdlet을 실행합니다. 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

또는 새 정책을 만들고 **-AllowCloudRecordingForCalls를** $true  정책을 사용자에게 할당할 수 있습니다. 

자세한 내용은 1:1 통화 기록 정책 [컨트롤은 거의(거의!)를 참조하세요. 여기에서 을(를)](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)클릭
