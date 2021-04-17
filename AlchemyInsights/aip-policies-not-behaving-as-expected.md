---
title: 'AIP: 정책이 예상대로 작동하지 않음'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821633"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: 정책이 예상대로 작동하지 않음

Azure Information Protection: 정책이 예상대로 작동하지 않습니다. 다양한 정책 문제에 대한 권장 지침은 다음을 참조하세요.

1. 시각적 표시에 문제가 있는 경우 [시각적 표시가 적용되는 경우](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)를 검토하세요.
2. 자동 레이블 지정에 문제가 있는 경우 [Azure Information Protection에 대한 자동 및 권장 분류 조건을 구성하는 방법](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) 및 [중요한 정보 유형이 찾는 항목](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)을 검토하세요.
3. 기본/Pfile 보호와 관련된 문제가 발생하는 경우 [파일 API 구성](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)을 검토하세요.
4. 올바르게 구성되지 않은 범위 지정 정책을 사용 중인지 확인합니다. [범위 지정된 정책을 사용하여 특정 사용자에 대한 Azure Information Protection 정책을 구성하는 방법](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)을 참조하세요.
5. 레이블이 지정된 문서를 첨부할 때 Outlook에서 자동 레이블 지정이 작동하지 않는 경우 여기에 설명된 대로 DRMEncryptProperty가 정의되어 있지 않은지 확인합니다. [보안용 IRM 레지스트리 설정](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

문제가 계속 발생하는 경우 Azure Information Protection 클라이언트 로그를 수집하고 내보낸 로그를 해당 티켓에 첨부하세요.

1. Office 문서를 열거나 Outlook에서 새 전자 메일을 작성합니다.
2. **보호/민감도** > **도움말 및 피드백** 을 클릭합니다.
3. **로그 내보내기** 를 클릭합니다.
4. 원하는 위치에 로그를 저장하고 해당 서비스 요청에 첨부합니다.

추가 리소스:

- [Azure Information Protection용 시각적 표시에 대한 레이블을 구성하는 방법](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure Information Protection 설명서 검토](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Microsoft 365 앱의 민감도 레이블 사용](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

