---
title: 기본 Outlook 레이블 설정이 적용되지 않습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/17/2021
ms.locfileid: "58370213"
---
# <a name="default-outlook-label-setting-not-applied"></a>기본 Outlook 레이블 설정이 적용되지 않습니다.

기본 Outlook 설정이 제대로 적용되지 않고 다른 레이블이나 레이블이 적용되지 않은 경우 알려진 문제(MC277818)가 발생하여 다음 두 옵션 중 하나를 사용하여 문제를 해결해야 합니다.

**옵션 1:**

1. Microsoft 365 센터 > **정보**  >  **보호로 이동하세요.**
1. 레이블 **정책 을** 선택하고 편집해야 하는 레이블 정책을 선택합니다(**OutlookDefaultlabel** 설정이 해당 레이블 정책에 제대로 설정되지 않았습니다. **Get-labelpolicy를** 실행하여 이 설정을 본 다음 정책 편집 **을 선택합니다.**
1. 정책 **설정** 대화 상자에서 사용자에게 레이블을 후속 전자 메일  및 문서에 적용해야 를 선택하면 사용할 수 있는 전자 메일에 이 기본 레이블 적용 설정이 표시될 때까지 **다음을** 선택합니다. 
1. 문서에 **기본** 레이블 적용 대화 상자의  드롭다운 목록에서 없음을 선택합니다.
1. 다음 **및** **제출을 선택하여** 레이블 설정을 저장합니다.

**옵션 2:**

보안 및 준수 센터 [Powershell에서](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)Set-LabelPolicy commandlet을 사용하여 {OutlookDefaultLabel="None"}에서 **OutlookDefaultlabel을** **None으로** 변경합니다.

실행: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

기본 레이블에 대한 자세한 Outlook 에 대해 다른 기본 레이블 [Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)