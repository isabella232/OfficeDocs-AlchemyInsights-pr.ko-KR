---
title: " eDiscovery 보류 오류 문제 해결"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 2a7372c7b20b87c8c774eae4ca4540a3bd19709596405da041eeaa24db310fa7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105394"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a> eDiscovery 보류 오류 문제 해결

eDiscovery 보류에 문제가 있나요? 다음은 고려할 몇 가지 모범 사례입니다.

- 보류 배포 상태를 검사합니다.  상태가 **켜짐(보류 중)** 혹은 **꺼짐(보류 중)** 인 경우 보류 배포가 완료될 때까지 기다립니다.
- 각 트랜잭션에 대해 정책을 반복적으로 업데이트하는 대신 eDiscovery 보류 업데이트를 단일 일괄 요청으로 병합합니다.
- 보안 및 준수 센터 PowerShell에서 Set-CaseHoldPolicy <policyname> -RetryDistribution을 실행합니다. 자세한 내용은 [보안 및 준수 센터 PowerShell에 연결](/powershell/exchange/connect-to-scc-powershell)을 참조하세요.

이러한 설정 및 eDiscovery 보류 문제를 완화하고 해결하는 추가 모범 사례를 확인하기 위한 단계는 [eDiscovery 보류 오류 문제 해결](/microsoft-365/compliance/hold-distribution-errors)을 참조하세요.
다른 일반적인 eDiscovery 문제 해결에 대한 자세한 내용은 [일반적인 eDiscovery 문제 조사, 문제 해결 및 해결](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)을 참조하세요.
