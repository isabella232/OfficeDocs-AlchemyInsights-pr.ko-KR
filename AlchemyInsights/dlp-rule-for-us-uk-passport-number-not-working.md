---
title: 미국/영국 여권 번호에 대한 DLP 규칙이 작동하지 않습니다.
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004952"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>DLP 문제 - 미국/영국 여권 번호

**중요**: 이 시기에는 SharePoint Online 및 OneDrive 서비스를 항상 사용할 수 있도록 하는 단계를 진행하고 있습니다. 자세한 내용은 [SharePoint Online 임시 기능 조정](https://aka.ms/ODSPAdjustments)을 참조하세요.

**미국/영국 여권 번호에 대한 DLP 문제**

O365에서 **DLP** 중요한 정보 유형을 사용할 때 **미국/영국** 여권 번호가 포함된 콘텐츠에 대해 DLP(데이터 손실 방지)가 작동하지 않는 문제가 있나요? 그렇다면 DLP 정책이 평가되는 경우 콘텐츠에 필요한 정보를 포함해야 합니다.
  
예를 들어 신뢰 수준이 75%인 **미국/영국** 여권 번호 정책의 경우 다음이 평가되고 규칙이 트리거될 때 검색되어야 합니다.
  
- **[형식:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 9자리 숫자

- **[패턴:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 9자리 연속 숫자

- **[체크 um:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** 아니요, 체크 um이 없습니다.

- **[정의:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP 정책은 300자 이내의 접근성으로 이러한 유형의 중요한 정보가 검색된 것으로 75% 확신합니다.

  - Func_usa_uk_passport 함수가 해당 패턴과 일치하는 콘텐츠를 찾습니다.

  - Keyword_passport의 키워드가 발견되었습니다.

    예를 들어 **미국/영국** 여권 번호 정책에 대해 트리거되는 샘플은 미국 여권 번호 123456789

콘텐츠에 대해 미국/영국 여권 번호가 검색되는 데 필요한 내용에 대한 자세한 내용은 이 문서의 다음 섹션을 참조하세요. [미국/영국](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) 여권 번호를 검색하는 중요한 정보 유형
  
다른 기본 제공 중요한 정보 유형을 사용하는 경우 다른 유형에 필요한 정보: 중요한 정보 유형이 찾아야 하는 사항 문서를 [참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  