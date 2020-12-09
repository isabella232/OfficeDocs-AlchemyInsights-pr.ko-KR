---
title: Microsoft Edge 개인 정보 설정 구성
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
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599513"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge 개인 정보 설정 구성

기본적으로 Microsoft Edge가 비 Windows 플랫폼에 배포된 경우 진단 데이터 및 사이트 정보가 Microsoft로 전송되지 않습니다. 그러나 Microsoft Edge가 Windows 10에 배포된 경우 사용자의 Windows 진단 데이터 설정에 따라 진단 데이터 및 사이트 [정보가 전송됩니다.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Microsoft Edge에서 조직의 데이터 수집을 처리하는 방법을 구성하기 위해 다음 그룹 정책을 사용 합니다.
- [MetricsReportingEnabled:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)이 정책은 사용 현황 및 크래시 관련 데이터를 보고할 수 있습니다.
- [SendSiteInfoToImproveServices:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)이 정책은 Microsoft 서비스를 개선하는 데 사용되는 사이트 정보를 전송합니다.

자세한 내용은 정책 설정 [구성을 참조하세요.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)