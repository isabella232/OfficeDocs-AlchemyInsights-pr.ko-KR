---
title: 하드 Microsoft Edge 경로 대신 데이터 디렉터리 변수를 사용하여 데이터 디렉터리 수정
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 235696d17711726da57d9a09c23b5b13140a28d7645299ef120a4b2c7b395c5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54113422"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>하드 Microsoft Edge 경로 대신 데이터 디렉터리 변수를 사용하여 데이터 디렉터리 수정

예를 들어 Windows의 경우 기본 위치가 아닌 사용자의 로컬 응용 프로그램 데이터에 프로필 데이터를 저장하려면 **UserDataDir** 정책을 **${local_app_data}\Edge\Profile** 로 설정합니다. 

자세한 내용은 [Create Microsoft Edge user data directory variables를 참조하십시오.](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)