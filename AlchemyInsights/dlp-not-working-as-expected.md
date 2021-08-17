---
title: DLP가 예상대로 작동하지 않습니다.
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079708"
---
# <a name="dlp-not-working-as-expected"></a>DLP가 예상대로 작동하지 않습니다.

**중요**: 이 시기에는 SharePoint Online 및 OneDrive 서비스를 항상 사용할 수 있도록 하는 단계를 진행하고 있습니다. 자세한 내용은 [SharePoint Online 임시 기능 조정](https://aka.ms/ODSPAdjustments)을 참조하세요.

 **DLP 설정**

DLP(데이터  손실 방지)에 문제가 Office 365 작동하지 않는 경우 그렇다면 **DLP** 정책이 올바르게 설정되어 있는지, 그리고 데이터에 평가할 때 **DLP** 정책이 찾고 있는 것이 포함되어 있는지 확인합니다.
  
DLP 정책을 사용하면 조직에서 중요한 정보를 식별하고 보호할 수 있습니다. DLP 정책을 설정하려면 에서 정보를 [사용하세요.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **DLP 정책이 찾아야 하는 것**
  
보안 및  규정 준수 센터에서 기본 제공 중요한 정보 유형을 사용하는 경우 DLP 정책은 이러한 중요한 유형을 검색할 때 특정 패턴 및 요소를 검색합니다.
  
- **기본 제공 중요한 정보 유형**

    기본 제공 중요한 유형 및 중요한 유형을 검색할 때 DLP 정책이 검색하는 내용은 다음을 참조하세요. 중요한 정보 유형이 검색하는 것을 [참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **사용자 지정 중요한 정보 유형**

    사용자 지정 중요한 정보 유형을 만들려고 하면 사용자 지정 중요한 정보 유형을 만드는 방법에 대한 자세한 내용은 사용자 지정 중요한 정보 유형 만들기 를 [참조하십시오.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**DLP 정책 테스트**

기본 제공 또는 사용자 지정 중요한 정보 유형으로  데이터를 테스트하기 위해 분류 중요한 정보 유형 에서 테스트 유형  >  **옵션을 사용합니다.** 자세한 내용은 사용자 지정 중요한 정보 [유형 테스트를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **보고서**
  
- DLP 보고서를 사용하여 중요한 [데이터 인사이트를 얻습니다.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- 인시던트 보고서 를 통해 이벤트의 특정 [세부 정보를 볼 수 있습니다.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
