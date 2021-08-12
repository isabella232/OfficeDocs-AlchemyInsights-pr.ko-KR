---
title: 민감도 레이블이 나타나지 않습니다.
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061438"
---
# <a name="sensitivity-labels-not-appearing"></a>민감도 레이블이 나타나지 않습니다.

민감도 레이블을 사용하면 중요한 콘텐츠를 분류하고 보호할 수 있습니다. 분류된 민감도 레이블의 Microsoft 365 규정 준수 센터, Microsoft 365 또는 Microsoft 365 & 규정 준수 센터에서 > 수 있습니다. 이 기능에 대한 자세한 내용은 민감도 레이블 [개요를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

민감도 레이블을 구성했지만 해당 레이블이 Microsoft 365 없는 경우 다음을 검사합니다.

- 민감도 레이블이 원하는 [](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) 사용자 및 그룹에 게시되어 있는지 확인

- 사용자가 민감도 레이블을 지원하는 앱을 사용하고 있는지 확인 - 문서에서 민감도 [레이블을 참조하세요.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- Azure Information [Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)레이블을 마이그레이션하는 경우 여기에 나열된 고려 사항을 알고 [있어야 합니다.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- DLP(데이터 손실 방지) 지원: 현재 보존 레이블만 DLP 정책의 조건으로 사용할 수 있습니다.  DLP 정책에서 민감도 레이블에 대한 지원은 아직 제공되지 않지만 현재 작업 중입니다.

- 민감도 레이블에서 암호화를 사용하도록 설정한 경우 다음 중 하나를 선택할 수 있습니다.
    - 지금 권한 할당
    - 사용자가 권한을 할당하도록 허용


가능한 문제에 대한 자세한 내용은 민감도 [레이블의 알려진 문제를 참조하세요.](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)