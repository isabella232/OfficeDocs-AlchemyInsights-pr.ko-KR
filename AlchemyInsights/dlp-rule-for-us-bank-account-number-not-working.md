---
title: 미국 은행 계좌 번호에 대한 DLP 규칙이 작동하지 않습니다.
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005024"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>미국 은행 계좌 번호에 대한 DLP 문제

**중요**: 이 시기에는 SharePoint Online 및 OneDrive 서비스를 항상 사용할 수 있도록 하는 단계를 진행하고 있습니다. 자세한 내용은 [SharePoint Online 임시 기능 조정](https://aka.ms/ODSPAdjustments)을 참조하세요.

**미국 은행 계좌 번호에 대한 DLP 문제**

O365에서 DLP 중요한 정보 유형을 사용할 때 **미국** 은행 계좌 번호가 포함된 콘텐츠에 대해 DLP(데이터 손실 **방지)가** 작동하지 않는 문제가 있나요? 그렇다면 DLP 정책이 평가되는 경우 콘텐츠에 필요한 정보를 포함해야 합니다.
  
예를 들어 신뢰 수준이 85%인 **미국** 은행 계좌 번호 정책의 경우 다음이 평가되고 규칙이 트리거될 수 있도록 검색되어야 합니다.
  
- **[형식:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17자리 숫자

- **[패턴:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17자리 연속 숫자

- **[체크 um:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** 아니요, 체크 um이 없습니다.

- **[정의:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP 정책은 300자 이내의 접근성으로 이러한 유형의 중요한 정보가 검색된 것으로 75% 확신합니다.

  - 정규식 Regex_usa_bank_account_number 일치하는 콘텐츠를 찾을 수 있습니다.

  - Keyword_usa_Bank_Account의 키워드가 발견되었습니다.

    예를 들어 다음 샘플은 **미국** 은행 계좌 번호 정책에 대해 트리거됩니다. Checking Account 78344011

콘텐츠에 대해 **미국** 은행 계좌 번호를 검색하는 데 필요한 내용에 대한 자세한 내용은 이 문서의 다음 섹션을 참조하세요. [](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) 미국 은행 계좌 번호를 검색하는 중요한 정보 유형
  
다른 기본 제공 중요한 정보 유형을 사용하는 경우 다른 유형에 필요한 정보: 중요한 정보 유형이 찾아야 하는 사항 문서를 [참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  