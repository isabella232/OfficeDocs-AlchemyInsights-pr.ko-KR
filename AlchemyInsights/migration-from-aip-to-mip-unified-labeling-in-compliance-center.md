---
title: 규정 준수 센터에서 AIP로부터 MIP/통합 레이블로 마이그레이션
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674332"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>규정 준수 센터에서 AIP로부터 MIP/통합 레이블로 마이그레이션

보안 및 규정 준수 센터에서 AIP 레이블로부터 통합 레이블로 마이그레이션하려면 다음을 실행합니다.

**Azure portal에서 보호 활성화**

1. 아직 실행하지 않은 경우 새 브라우저 창을 열고 [Azure portal에 로그인](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)합니다. **Azure Information Protection** 블레이드를 탐색합니다. 예를 들어 허브 메뉴에서 **모든 서비스**를 클릭하고 필터 상자에 **정보**를 입력합니다. **Azure Information Protection**을 선택합니다. 전에 Azure Information Protection 블레이드에 액세스한 적이 없는 경우 일회성의 [추가 단계](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time)를 참조하여 포털에 블레이드를 추가하세요. Azure Information Protection 블레이드를 열려면 [Azure Information Protection 프리미엄 플랜](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) 또는 권한 관리가 포함된 Office 365 플랜이 있어야 합니다. 구독 중 하나를 이용하고 있지만 유효한 구독을 찾을 수 없다는 메시지가 표시되면 [Microsoft 지원에 문의](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support)하거나 기본 지원 채널을 이용하세요.

2. **관리** 메뉴 옵션을 찾고 **보호 활성화**를 선택합니다. **활성화**를 클릭한 후 작업을 확인합니다. 활성화가 완료되면 정보 표시줄에 **활성화가 성공적으로 완료되었습니다**라는 문구가 표시됩니다.

**Azure Information Protection 레이블을 Office 365 보안 및 준수 센터로 마이그레이션**

1. 전역 관리자 권한을 가진 사용자로 로그인했는지 확인합니다.

2. **Azure Information Protection** 블레이드를 탐색합니다.

3. **관리** 메뉴 옵션에서 **통합 레이블**을 선택합니다.

4. **Azure Information Protection-통합 레이블** 블레이드에서 **활성화**를 클릭하고 온라인 지침을 따릅니다.

**참고**: 보안 및 준수 센터 마이그레이션을 활성화하기 전에 적합한 사용 권한이 있는지 확인하세요. 자세한 내용은 다음 문서를 참조하세요.

1. [Azure Information Protection을 구성하기 위해서는 전역 관리자가 되야 하나요? 아니면 다른 관리자에게 위임할 수 있나요?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [보안 및 준수 센터로 마이그레이션한 후 관리자 역할에 대한 중요 정보](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

보안 및 규정 준수 센터 내 AIP에서 통합 레이블로 마이그레이션 관련하여 자세한 내용은 [레이블 마이그레이션](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels) 참조하세요.
