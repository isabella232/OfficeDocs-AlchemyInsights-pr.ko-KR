---
title: DLP가 예상 대로 작동 하지 않음
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
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679699"
---
# <a name="dlp-not-working-as-expected"></a>DLP가 예상 대로 작동 하지 않음

**중요**: 이 시기에는 SharePoint Online 및 OneDrive 서비스를 항상 사용할 수 있도록 하는 단계를 진행하고 있습니다. 자세한 내용은 [SharePoint Online 임시 기능 조정](https://aka.ms/ODSPAdjustments)을 참조하세요.

 **DLP 설정**

Office 365에서 **DLP (데이터 손실 방지)** 에 대 한 문제가 예상 대로 작동 하지 않습니까? 이 경우 **dlp 정책이** 올바르게 설정 되어 있고 데이터에 **dlp 정책이** 평가 되는 동안 검색 하는 작업이 포함 되어 있는지 확인 합니다.
  
DLP 정책을 사용 하면 조직의 중요 한 정보를 식별 하 고 보호할 수 있습니다. DLP 정책을 설정 하려면 [여기](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)에서 정보를 사용 합니다.
  
 **DLP 정책에서 찾는 사항**
  
보안 및 준수 센터에서 **기본 제공 중요 한 정보 유형을** 사용 하는 경우 DLP 정책은 이러한 중요 한 유형을 검색할 때 특정 패턴 및 요소를 찾습니다.
  
- **기본 제공 중요 한 정보 유형**

    기본 제공 중요 한 유형과 중요 한 유형을 검색할 때 DLP 정책에서 찾는 사항에 대 한 자세한 내용은 [중요 한 정보 유형에서 찾는 항목](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)을 참조 하십시오.

- **사용자 지정 중요 한 정보 유형**

    사용자 지정 중요 한 정보 유형을 만들려는 경우에는 사용자 지정 중요 한 [정보](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)유형을 만드는 방법에 대 한 자세한 내용은 다음 문서를 참조 하십시오.

**DLP 정책 테스트**

기본 제공 또는 사용자 지정 중요 한 정보 유형을 사용 하 여 데이터를 테스트 하려면 **분류**중요 정보 유형에 서 **테스트 유형** 옵션을 사용  >  **Sensitive info types**합니다. 자세한 내용은 [사용자 지정 중요 한 정보 유형 테스트](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)를 참조 하세요.

 **보고서**
  
- DLP 보고서를 사용 하 여 중요 한 데이터를 파악 [합니다.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- 이벤트에 대 한 구체적인 세부 정보를 [문제 보고서](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)와 함께 참조 하십시오.
