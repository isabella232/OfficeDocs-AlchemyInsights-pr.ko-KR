---
title: Linux 컴퓨터의 MDATP 제외 구성 및 유효성 검사
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568617"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a>Linux 컴퓨터의 MDATP 제외 구성 및 유효성 검사

MDATP 검사에서 특정 파일, 폴더, 프로세스 및 처리된 파일을 제외할 수 있습니다. 제외는 조직에 고유하거나 사용자 지정된 소프트웨어 및 파일을 잘못 검색하지 못하도록 방지하는 데 도움이 됩니다. 제외는 MDATP로 인한 성능 문제를 완화하는 데도 도움이 됩니다.

자세한 내용은 [Linux용 MDATP에](https://go.microsoft.com/fwlink/?linkid=2144517)대한 제외 구성 및 유효성 검사를 참조합니다.

> [!IMPORTANT]
> 이 문서에 설명된 제외는 끝점 감지 및 응답(EDR)을 포함하여 Linux용 MDATP의 다른 기능에는 적용되지 않습니다. 이 문서에 설명된 방법을 사용하여 제외하는 파일은 여전히 EDR 경고 및 기타 검색 기능을 트리거할 수 있습니다.
