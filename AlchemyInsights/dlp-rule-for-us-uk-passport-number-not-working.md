---
title: US/영국 여권 번호가 작동 하지 않는 DLP 규칙
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507304"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>DLP-US/영국 여권 번호 관련 문제

**중요**: 이 시기에는 SharePoint Online 및 OneDrive 서비스를 항상 사용할 수 있도록 하는 단계를 진행하고 있습니다. 자세한 내용은 [SharePoint Online 임시 기능 조정](https://aka.ms/ODSPAdjustments)을 참조하세요.

**US/영국 여권 번호와 관련 된 DLP 문제**

O365에서 DLP 중요 한 정보 유형을 사용할 때 **US/영국 여권 번호가** 포함 된 콘텐츠에 대해 **Dlp (데이터 손실 방지)** 가 작동 하지 않는 문제를 겪고 있습니까? 이 경우 콘텐츠를 평가할 때 필요한 DLP 정책에 대 한 정보가 포함 되어 있는지 확인 합니다.
  
예를 들어 **미국/영국 여권 번호** 정책의 신뢰 수준이 75% 인 경우 다음이 평가 되며 규칙을 트리거하기 위해 검색 되어야 합니다.
  
- **[형식:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 9 자리 숫자

- **[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 9 자리 연속 숫자

- **[검사 값:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** 아니요, 체크섬이 없습니다.

- **[정의:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP 정책은 300 문자에 근접 한 경우이 유형의 중요 한 정보를 검색 한다는 것을 75% 확신 합니다.

  - Func_usa_uk_passport 함수가 해당 패턴과 일치하는 콘텐츠를 찾습니다.

  - Keyword_passport의 키워드가 발견되었습니다.

    예를 들어 미국 여권 번호 123456789에 대 한 다음 샘플은 **US/영국 여권 번호** 정책에 대해 트리거됩니다.

콘텐츠에 대 한 US/영국 여권 번호를 검색 하는 데 필요한 사항에 대 한 자세한 내용은이 문서의 다음 섹션에서 [중요 한 정보 유형이 US/Uk Passport 번호에 대해 어떻게 나타나는지](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) 를 참조 하세요.
  
기본 제공 되는 다른 중요 한 정보 유형을 사용 하는 경우 [중요 한 정보 유형이 찾는 항목](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) 에 대 한 자세한 내용은 다음 문서를 참조 하십시오.
  