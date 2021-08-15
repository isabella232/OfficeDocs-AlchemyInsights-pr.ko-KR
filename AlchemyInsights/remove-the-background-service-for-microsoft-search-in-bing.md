---
title: Bing에서 Microsoft Search의 배경 서비스 제거
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 07d24290fc3b13cce7a931c4cff15176c080b4413489ba1935b6886939ea3874
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53982379"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Bing에서 Microsoft Search의 배경 서비스 제거

Bing에서 Microsoft Search의 배경 서비스를 제거하려면 다음 방법을 시도해 볼 수 있습니다.

1. 원래 검색 엔진 설정으로 되돌리려면 다음 작업을 수행하세요.

    a. **Bing을 기본 검색 엔진으로 사용 [ 토글을](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)끄기** 로 전환합니다.

    b. [Microsoft 365 관리 센터로 이동](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed)하여조직의 모든 사용자에게 영향을 주는 설정을 삭제합니다.

2. 개별 장치에서 배경 서비스를 제거하려면 다음 작업을 수행하세요.

    a. **제어판 > 프로그램 > 프로그램 및 기능** 을 선택합니다.

    b. 설치된 프로그램 목록에서 **Bing의 Microsoft Search** 를 마우스 오른쪽 단추로 클릭한 다음 **제거** 를 클릭합니다.

3. 조직의 여러 장치에서 배경 서비스를 제거하려면 관리자로 로그인하고 스크립트에서 다음 명령을 실행합니다. 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
