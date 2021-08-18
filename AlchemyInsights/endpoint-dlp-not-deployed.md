---
title: 엔드포인트 DLP가 사용자의 장치에 배포되지 않음
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: fa0e2766e1526d8e81cb247029e7c0fd98630b96
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316824"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>엔드포인트 DLP가 사용자의 장치에 배포되지 않음

엔드포인트 데이터 손실 방지(DLP) 설정이 사용자의 장치에 적용되지 않은 경우 다음 요구 사항을 충족하는지 확인하세요.

- Windows 10 x64 빌드 1809 이상이 장치에 설치되어 있습니다.
- 맬웨어 방지 클라이언트 버전 4.18.2009.7 이상이 설치되어 있습니다.
- 장치가 다음 중 **하나** 입니다.
    
    - Azure AD(Azure Active Directory) 조인됨
    - 하이브리드 Azure AD 조인됨
    - AAD 등록됨

- 클라우드로 업로드 활동에 대한 정책 작업을 적용하려면, 엔드포인트 장치에 Microsoft Chromium Edge 브라우저를 설치하세요.

Endpoint DLP 배포에 대한 추가 요구 사항은 [Endpoint 데이터 손실 방지 시작하기](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)를 참조하세요.