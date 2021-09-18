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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446697"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP에 사용자 지정 유형이 필요할 수 있습니다.

**중요**: 이 시기에는 SharePoint Online 및 OneDrive 서비스를 항상 사용할 수 있도록 하는 단계를 진행하고 있습니다. 자세한 내용은 [SharePoint Online 임시 기능 조정](https://aka.ms/ODSPAdjustments)을 참조하세요.

**DLP에 사용자 지정 정보 유형이 필요할 수 있습니다.**

DLP(데이터 손실 방지) 정책을 사용하면 조직의 중요한 데이터를 식별하고 보호할 수 있습니다. 일부 시나리오에서는 조직의 데이터를 보호하기 위해 사용자 지정 중요한 정보 유형을 직접 만들어야 할 수 있습니다. 자세한 내용은 [중요한](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) 정보 유형 및 중요한 정보 유형 엔터티 [정의에 대한 자세한 정보를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

사용자 지정 중요한 정보 유형 및 정책을 만드는 방법에 대한 자세한 내용은 다음을 참조하세요. 

**기본으로 제공되는 중요한 정보 유형 사용자 지정**

몇 가지 조정만 하여 기본 제공 중요한 정보 유형이 요구 사항을 충족하는 경우 기본 제공 중요한 정보 유형 사용자 [지정을 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) 예를 들어 키워드를 추가 또는 제거하거나 날짜 또는 주소와 같은 지원 증거를 추가하거나 제거할 수 있습니다.

**사용자 지정 중요한 정보 유형 만들기**

그러나 서로 다른 유형의 중요한 정보를 모두 식별하고 보호해야 하는 경우 중요한 정보 유형에 사용자 지정 중요한 정보 유형을 Microsoft 365 규정 준수 센터. 자세한 내용은 사용자 지정 중요한 정보 [유형 시작을 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**보안 및 준수 센터 PowerShell에서 사용자 지정 중요한 정보 유형 만들기**

마지막으로 사용자 인터페이스가 필요한 모든 옵션을 제공하지 않는 경우 보안 및 준수 센터 PowerShell에서 사용자 지정 중요한 정보 유형을 & 있습니다. XML 파일로 시작하면 사용 가능한 모든 옵션을 사용할 수 있습니다. 자세한 내용은 PowerShell을 사용하여 사용자 지정 중요한 [정보 유형 만들기를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)

먼저 테스트 모드에서 정책을 테스트하는 [](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) 경우 테스트 모드에서 정책 구현 및 DLP 정책 만들기, 테스트 및 [조정을 참조합니다.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 