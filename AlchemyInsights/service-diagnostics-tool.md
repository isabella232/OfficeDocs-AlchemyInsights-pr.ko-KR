---
title: Windows Virtual Desktop용 서비스 진단 도구
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: e6c20af2c3fc54b203f3bda5c0c0f00faacd92800566bd507867c4e9fe4a23f1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052320"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Windows Virtual Desktop용 서비스 진단 도구

WVD(Windows Virtual Desktop)는 관리자가 단일 인터페이스를 통해 오류를 식별할 수 있는 진단 도구를 제공합니다. 이 도구는 WVD 역할을 할당한 사용자가 WVD를 사용할 때마다 진단 관련 정보를 기록합니다. 각 로그에는 활동에 포함된 WVD 역할에 대한 정보, 세션 중에 나타나는 오류 메시지, 테넌트 및 사용자에 대한 정보가 포함됩니다. Azure Log Analytics는 다음 단계를 수행하여 진단 도구가 생성한 작업 로그를 캡처하도록 구성할 수 있습니다.

1. [Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) 또는 [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)을 사용하여 Log Analytics 작업 영역을 만듭니다.

1. [Windows 컴퓨터를 Azure Monitor에 연결합니다](https://go.microsoft.com/fwlink/?linkid=2129913). 작업 영역 ID와 작업 영역의 기본 키를 받습니다. 에이전트를 올바르게 구성하고 Azure Monitor와 통신할 수 있도록 하려면 설정 마법사에서 이 정보가 필요합니다.

1. [진단 데이터를 작업영역에 푸시합니다](https://go.microsoft.com/fwlink/?linkid=2128284). WVD 테넌트에서 작업 영역의 진단 데이터를 Log Analytics에 푸시할 수 있습니다.

1. WVD와 관련된내부 또는 외부 문제를 [식별하고 진단](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)합니다.

WVD용 서비스 진단 도구를 구성하는 방법에 대한 자세한 내용은 진단 기능에 대한 Log Analytics 사용을 참조하세요.