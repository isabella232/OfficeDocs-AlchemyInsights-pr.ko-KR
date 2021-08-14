---
title: 신용 카드 번호에 대한 DLP 규칙이 작동하지 않습니다.
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005096"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>신용 카드 번호에 대한 DLP 문제

**중요**: 이 시기에는 SharePoint Online 및 OneDrive 서비스를 항상 사용할 수 있도록 하는 단계를 진행하고 있습니다. 자세한 내용은 [SharePoint Online 임시 기능 조정](https://aka.ms/ODSPAdjustments)을 참조하세요.

**신용 카드 번호에 대한 DLP 문제**

O365에서 DLP 중요한 정보 유형을 사용할 때  신용 카드 번호가 포함된 콘텐츠에 대해 DLP(데이터 손실 **방지)가** 작동하지 않는 문제가 있나요? 그렇다면 콘텐츠가 평가될 때 DLP 정책을 트리거하는 데 필요한 정보를 포함해야 합니다. 예를 들어 신뢰 수준이 85%인 **신용** 카드 정책의 경우 다음이 평가되고 규칙이 트리거될 때 검색되어야 합니다.
  
- **[형식:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 서식이 지정되거나 서식이 없는 16자리 숫자(dddddd)를 입력하고 Luhn 테스트를 통과해야 합니다.

- **[패턴:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Visa, MasterCard, Discover Card, JCB, American Express, 기프트 카드 및 다이너 카드를 비롯한 전 세계 모든 주요 브랜드의 카드를 감지하는 매우 복잡하고 강력한 패턴입니다.

- **[체크 um:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** 예, Luhn 체크 um

- **[정의:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP 정책은 300자 이내의 접근성으로 이러한 유형의 중요한 정보가 검색된 것으로 85% 확신합니다.

  - Func_credit_card 함수가 해당 패턴과 일치하는 콘텐츠를 찾습니다.

  - 다음 중 하나가 충족됩니다.

  - Keyword_cc_verification의 키워드가 발견되었습니다.

  - 검색된 Keyword_cc_name 발견

  - Func_expiration_date 함수가 올바른 날짜 형식의 날짜를 찾습니다.

  - 체크 체크 um이 통과

    예를 들어 다음 샘플은 DLP 신용 카드 번호 정책에 대해 트리거됩니다.

  - Visa: 4485 3647 3952 7352
  
  - 만료 날짜: 2009년 2월

콘텐츠에 대해 신용 카드  번호를 검색하는 데 필요한 내용에 대한 자세한 내용은 이 문서의 다음 섹션을 참조하세요. 중요한 정보 유형이 신용 카드를 검색하는 [내용#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
다른 기본 제공 중요한 정보 유형을 사용하는 경우 다른 유형에 필요한 정보: 중요한 정보 유형이 찾아야 하는 사항 문서를 [참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  