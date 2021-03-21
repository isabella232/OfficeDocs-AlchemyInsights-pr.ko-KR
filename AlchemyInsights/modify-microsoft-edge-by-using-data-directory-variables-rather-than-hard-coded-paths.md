---
title: 하드 코드된 경로가 아닌 데이터 디렉터리 변수를 사용하여 Microsoft Edge 수정
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897894"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>하드 코드된 경로가 아닌 데이터 디렉터리 변수를 사용하여 Microsoft Edge 수정

예를 들어 Windows의 경우 기본 위치가 아닌 사용자의 로컬 응용 프로그램 데이터에 프로필 데이터를 저장하려면 *UserDataDir* 정책을 **${local_app_data}\Edge\Profile** 로 설정합니다.

자세한 내용은 [Microsoft Edge 사용자 데이터 디렉터리 변수 만들기](https://docs.microsoft.com/deployedge/microsoft-edge-policies)를 참조하세요.