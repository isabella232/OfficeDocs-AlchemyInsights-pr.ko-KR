---
title: DLP에 사용자 지정 형식이 필요할 수 있음
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507520"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP에 사용자 지정 형식이 필요할 수 있음

**중요**: 이 시기에는 SharePoint Online 및 OneDrive 서비스를 항상 사용할 수 있도록 하는 단계를 진행하고 있습니다. 자세한 내용은 [SharePoint Online 임시 기능 조정](https://aka.ms/ODSPAdjustments)을 참조하세요.

**DLP에는 사용자 지정 정보 유형이 필요할 수 있습니다.**

DLP (데이터 손실 방지) 정책을 사용 하 여 조직에서 중요 한 데이터를 식별 하 고 보호할 수 있습니다. 일부 시나리오에서는 조직의 데이터를 보호 하기 위해 **사용자 지정** 중요 한 정보 유형을 직접 만들어야 할 수도 있습니다.

예를 들어 조직에서 조직의 특정 형식으로 직원 Id 또는 기타 데이터를 식별 하 고 보호 해야 할 수 있습니다. 이 경우 자세한 내용은 다음 문서를 참조 하세요.
  
 **기본 제공 중요한 정보 유형 사용자 지정**
  
기본 제공 중요 한 정보 유형이 몇 가지 수단 만으로 요구 사항을 충족 하는 경우 [에는 기본 제공 중요 한 정보 유형을 사용자 지정할](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)수 있습니다. 예를 들어 키워드를 추가 또는 제거 하거나, 날짜나 주소와 같은 지원 증거를 추가 하거나 제거할 수 있습니다.
  
 **사용자 지정 중요한 정보 유형 만들기**
  
그러나 서로 다른 유형의 중요 한 정보를 식별 하 고 보호 해야 하는 경우에는 보안 & 준수 센터의 UI에서 [사용자 지정 중요 한 정보 유형을 만들](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) 수 있습니다.
  
**보안 및 준수 센터 PowerShell에서 사용자 지정 중요한 정보 유형 만들기**

마지막으로 UI가 필요한 모든 옵션을 제공 하지 않는 경우 [보안 & 준수 센터 PowerShell에서 사용자 지정 중요 한 정보 유형을 만들](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)수 있습니다. XML 파일을 시작 하 여 사용 가능한 모든 옵션을 사용할 수 있습니다.
