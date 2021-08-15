---
title: AIP 클라이언트에서 자동 분류가 예상대로 작동하지 않음
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
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979715"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>AIP 클라이언트에서 자동 분류가 예상대로 작동하지 않음

자동 분류가 예상대로 작동하지 않는 경우 다음 권장 지침을 사용하세요.

1. 자동 레이블 지정에 문제가 있는 경우 [Azure Information Protection에 대한 자동 및 권장 분류 조건을 구성하는 방법](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) 및 [중요한 정보 유형이 찾는 항목](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)을 참조하세요.
2. 올바르게 구성되지 않은 범위 지정 정책을 사용 중인지 확인합니다. [범위 지정된 정책을 사용하여 특정 사용자에 대한 Azure Information Protection 정책을 구성하는 방법](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)을 참조하세요.
3. 레이블이 지정된 문서를 연결할 때 Outlook에서 자동 레이블 지정이 작동하지 않는 경우 여기에 설명된 것과 같이 `DRMEncryptProperty`이(가) 정의되어 있지 않은지 확인합니다. [보안용 IRM 레지스트리 설정](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. Azure Information Protection 정책의 [기본 제공 정보 유형](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b)을 사용한 경우 콘텐츠가 예상한 형식과 일치하는지 확인합니다.
5. 레이블이 **자동** 또는 **권장** 설정에 맞게 적절히 구성되었는지 확인합니다. **자동** 레이블 지정은 모든 Microsoft 365 앱에서 사용할 수 있지만, **권장** 설정은 Outlook을 제외한 모든 Microsoft 365 앱에서 사용할 수 있습니다.
6. 이전에 수동으로 레이블을 지정했거나, 이전에 상위 분류로 레이블이 자동으로 지정된 문서 및 전자 메일에는 자동 분류를 사용할 수 없습니다.  자세한 내용은 [자동 또는 권장 레이블이 적용되는 방식](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)을 참조하세요.
7. 문제가 계속 발생하는 경우 Azure Information Protection 클라이언트 로그를 수집하고 내보낸 로그를 지원 티켓에 첨부하세요. Azure Information Protection 로그를 내보내려면 다음을 수행합니다.
    - Office 문서를 열거나 Outlook에서 새 전자 메일을 작성합니다.
    - **보호/민감도** > **도움말 및 피드백** 을 클릭합니다.
    - **로그 내보내기** 를 클릭합니다.
    - 원하는 위치에 로그를 저장하고 서비스 요청에 첨부합니다.

자세한 내용은 다음 항목을 참조하세요.

- [Azure Information Protection에 대한 자동 및 권장 분류 조건을 구성하는 방법](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Azure Information Protection을 사용하는 일반적인 시나리오에 대한 방법 가이드](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Azure Information Protection 설명서 검토](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure Information Protection 구독 및 기능 검토](https://azure.microsoft.com/pricing/details/information-protection)
- [Azure Information Protection에 대한 요구 사항](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure Information Protection에 대한 빠른 시작 튜토리얼](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Azure Information Protection 클라이언트 다운로드](https://www.microsoft.com/download/details.aspx?id=53018)
