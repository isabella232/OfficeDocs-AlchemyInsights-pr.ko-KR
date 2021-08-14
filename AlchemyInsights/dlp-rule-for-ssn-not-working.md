---
title: SSN에 대한 DLP 규칙이 작동하지 않습니다.
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004988"
---
# <a name="dlp-issues-with-social-security-numbers"></a>주민 번호와 관련한 DLP 문제

**중요**: 이 시기에는 SharePoint Online 및 OneDrive 서비스를 항상 사용할 수 있도록 하는 단계를 진행하고 있습니다. 자세한 내용은 [SharePoint Online 임시 기능 조정](https://aka.ms/ODSPAdjustments)을 참조하세요.

**SSNS의 DLP 문제**

DLP(데이터 손실 **방지)가** **SSN(사회** 보장 번호)을 포함하는 콘텐츠에 대해 작동하지 않는 문제가 Microsoft 365. 그렇다면 콘텐츠에 DLP 정책의 내용에 필요한 정보가 포함되어 있는지 확인하세요. 
  
예를 들어 신뢰 수준이 85%인 SSN 정책의 경우 다음이 평가되고 규칙이 트리거될 수 있도록 검색되어야 합니다.
  
- **[형식:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 서식이 지정되거나 서식 없는 패턴일 수 있는 9자리 숫자

- **[패턴:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 4개의 함수는 네 가지 다른 패턴에서 SSNS를 찾아보세요.

  - Func_ssn 대시 또는 공백으로 서식이 지정되어 있는 2011년보다 강력한 서식이 있는 SSNS를 검색합니다(ddd-dd-dd-dddd OR ddd dddd).

  - Func_unformatted_ssn 9자리 연속 숫자로 서식이 지정되지 않은 강력한 2011 강력한 서식의 SSNS를 검색합니다(dddddddddd).

  - Func_randomized_formatted_ssn 공백(ddd-dd-dddd OR ddd d)으로 서식이 지정된 2011년 후 SSNS를 검색합니다.

  - Func_randomized_unformatted_ssn 9자리 연속 숫자로폼이 없는 2011년 후 SSNS를 검색합니다(dddddddd).

- **[체크 um:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** 아니요, 체크 um이 없습니다.

- **[정의:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP 정책은 300자 이내의 접근성으로 이러한 유형의 중요한 정보가 검색된 것으로 85% 확신합니다.

  - 이 [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) 패턴과 일치하는 콘텐츠를 검색합니다.

  - [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn)의 키워드가 발견되었습니다. 키워드의 예로는 *Social Security, Social Security#, Soc Sec ,SSN이 있습니다.* 예를 들어 DLP SSN 정책에 대해 **SSN: 489-36-8350** 샘플이 트리거됩니다.
  
콘텐츠에 대해 SSNS를 검색하는 데 필요한 내용에 대한 자세한 내용은 이 문서의 다음 섹션을 [참조하세요. SSNS를](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn) 검색하는 중요한 정보 유형
  
다른 기본 제공 중요한 정보 유형을 사용하는 경우 다른 유형에 필요한 정보: 중요한 정보 유형이 찾아야 하는 사항 문서를 [참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  