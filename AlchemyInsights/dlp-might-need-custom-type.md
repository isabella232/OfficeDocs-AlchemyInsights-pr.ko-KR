---
title: DLP에 사용자 지정 유형이 필요할 수 있습니다.
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030800"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP에 사용자 지정 유형이 필요할 수 있습니다.

**중요**: 이 시기에는 SharePoint Online 및 OneDrive 서비스를 항상 사용할 수 있도록 하는 단계를 진행하고 있습니다. 자세한 내용은 [SharePoint Online 임시 기능 조정](https://aka.ms/ODSPAdjustments)을 참조하세요.

**DLP에 사용자 지정 정보 유형이 필요할 수 있습니다.**

DLP(데이터 손실 방지) 정책을 사용하면 조직의 중요한 데이터를 식별하고 보호할 수 있습니다. 일부 시나리오에서는 조직의 데이터를 보호하기  위해 사용자 지정 중요한 정보 유형을 직접 만들어야 할 수 있습니다.

예를 들어 조직에서 조직에 특정한 형식의 직원 식별 및 보호를 해야 할 수 있습니다. 그렇다면 다음 문서를 참조하세요.
  
 **기본으로 제공되는 중요한 정보 유형 사용자 지정**
  
몇 가지 조정으로 기본 제공 중요한 정보 유형이 요구 사항을 충족하는 경우 기본 제공 중요한 정보 유형 을 사용자 지정할 [수 있습니다.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) 예를 들어 키워드를 추가 또는 제거하거나 날짜 또는 주소와 같은 지원 증거를 추가하거나 제거할 수 있습니다.
  
 **사용자 지정 중요한 정보 유형 만들기**
  
그러나 다른 유형의 중요한 정보를 모두 식별하고 보호해야 하는 경우 [](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) 보안 및 준수 센터의 UI에 사용자 지정 중요한 정보 유형을 & 있습니다.
  
**보안 및 준수 센터 PowerShell에서 사용자 지정 중요한 정보 유형 만들기**

마지막으로 UI가 필요한 모든 옵션을 제공하지 않는 경우 보안 및 준수 센터 [PowerShell에서](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)사용자 지정 중요한 정보 유형을 & 수 있습니다. XML 파일로 시작하면 사용 가능한 모든 옵션을 사용할 수 있습니다.
