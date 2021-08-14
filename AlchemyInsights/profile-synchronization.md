---
title: 프로필 동기화
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923650"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>내 프로필 변경 내용이 사용자 프로필 응용 프로그램과 SharePoint 동기화되는 경우

SharePoint 온라인에서는 AD 가져오기(Active Directory 가져오기) 작업을 사용하여 사용자 및 그룹을 사용자 프로필 응용 프로그램으로 가져올 수 있습니다. 
  
1. AD 가져오기에서는 SharePoint 온라인 디렉터리 저장소의 변경 내용을 사용자 프로필 응용 프로그램으로 동기화합니다. 이러한 변경 내용은 일괄 처리됩니다.
    
2. 변경 내용이 동기화될 때까지는 Timer 작업이 실행됩니다.
    
> [!NOTE]
> 작업이 실행되는 데 걸리는 시간은 처리에 대한 변경 내용의 수에 따라 달라 니다. 많은 변경 내용이 더 오래 소요됩니다. SLA(서비스 수준 계약)에는 SharePoint Online Directory의 사용자에 대한 변경이 24시간 후 사용자 프로필 응용 프로그램에 반영됩니다. 
  
[온라인에서 사용자 프로필 동기화에 대한 SharePoint 정보](https://go.microsoft.com/fwlink/?linkid=875671)
  

