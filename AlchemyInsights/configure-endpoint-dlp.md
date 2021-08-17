---
title: 끝점 DLP 구성
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 4a4dbd60f98e86cf2a4d861a763f75ada04f9e500164c01cb858a1537148a62f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892805"
---
# <a name="configure-endpoint-dlp"></a>끝점 DLP 구성

Microsoft 끝점 DLP를 사용하여 Windows 10 장치의 중요한 정보에 대한 DLP 보호 및 모니터링 기능을 확장할 수 있습니다. 장치를 장치 관리에 등록한 후 DLP 정책을 만들어 항목에 보호 작업을 적용할 수 있습니다. 활동 탐색기를 사용하여 중요한 항목의 활동을 모니터링할 수 있습니다. 자세한 내용은 [장치 관리에 장치 등록](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)을 참조하세요.  

끝점 DLP를 시작하려면 다음을 수행하세요.

- 해당 SKU/구독 라이선스가 있는지 확인합니다. 자세한 내용은 [SKU/구독 라이선스](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)를 참조하세요.
- 장치 관리를 사용하도록 설정하고 등록 페이지에 액세스하거나 장치 모니터링을 설정/해제하는 데 필요한 권한을 확인합니다. 자세한 내용은 [권한](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)을 참조하세요.
- 장치 등록 절차를 따라 장치 관리에 장치를 등록합니다. 자세한 내용은 [장치 등록](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)을 참조하세요. 
- DLP 정책을 만들어 중요한 항목을 보호합니다. 자세한 내용은 [끝점 DLP 정책 시나리오](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)를 참조하세요.

Microsoft 끝점 DLP에 대한 자세한 내용은 [Microsoft 365 끝점 데이터 손실 방지(미리 보기) 알아보기](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)를 참조하세요.

**지원이 필요한 경우 중요한 데이터 수집 단계:**

1. [MDATP 클라이언트 분석기 미리 보기](https://aka.ms/betamdatpanalyzer)를 다운로드합니다.
1. cmd 창에서 도구를 관리자로 실행합니다.

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. **추적을 수집할 시간(분) 입력:** 메시지가 표시되면 시나리오를 실행하는 데 필요한 시간(분)을 입력합니다.
1. 시나리오를 실행합니다.

지원 에이전트에 제공할 Zip 파일 출력을 수집합니다.
