---
title: Teams가 시작되지 않음
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100225"
---
# <a name="teams-doesnt-launch"></a>Teams가 시작되지 않음

Microsoft Teams를 열려고 하지만 시작되지 않는 경우 다음을 시도해 보세요.

1. **%appdata%\Microsoft\Teams** 로 이동합니다.
1. 폴더의 내용을 삭제합니다.
1. 컴퓨터를 다시 시작하고 Teams를 실행합니다.

Teams를 다시 설치해야 할 수도 있습니다. 다시 설치하려면 다음을 수행하세요.

1. 제어판 사용하여 Teams를 제거합니다.
1. **%appdata%\Microsoft\Teams\Application 캐시** 로 이동합니다.
1. 폴더의 내용을 삭제합니다.
1. **%appdata%\Microsoft\teams\Cache** 로 이동합니다.
1. 폴더의 내용을 삭제합니다.
1. 컴퓨터를 다시 시작한 다음 Teams를 다운로드하여 설치합니다.

로그인할 수 없는 특정 사용자에 대해 테넌트에서 진단을 실행하려면 **TeamsUserUnableToSignIn** 키워드를 사용하여 새 검색을 시작하고 프롬프트를 따릅니다.