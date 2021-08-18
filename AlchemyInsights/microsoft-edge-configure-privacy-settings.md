---
title: Microsoft Edge 설정 구성
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114178"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge 설정 구성

기본적으로 Microsoft Edge 플랫폼에 Windows 경우 진단 데이터 및 사이트 정보가 Microsoft로 전송되지 않습니다. 그러나 Microsoft Edge 배포된 Windows 10 진단 데이터 및 사이트 정보는 사용자의 진단 데이터 설정에 따라 [Windows 전송됩니다.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

조직의 데이터 Microsoft Edge 처리하는 방법을 구성하기 위해 다음 그룹 정책을 사용 합니다.
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): 이 정책은 사용 현황 및 크래시 관련 데이터를 보고할 수 있습니다.
- [SendSiteInfoToImproveServices:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)이 정책은 사이트 정보를 개선하는 데 사용되는 사이트 Microsoft 서비스.

자세한 내용은 정책 설정 [구성을 참조하세요.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)