---
title: Privileged Identity Management 역할
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973235"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM) 역할

**역할을 활성화한 후 사용 권한이 부여되지 않습니다.**

Azure AD PIM(Privileged Identity Management)에서 역할을 활성화하면 권한 있는 역할이 필요한 모든 포털에 정품 인증이 즉시 전파되지 않을 수 있습니다. 경우에 따라 변경이 전파된 경우에도 포털의 웹 캐싱으로 인해 변경이 즉시 적용되지 않을 수 있습니다.

정품 인증이 지연되는 경우 다음 단계를 수행합니다.

1. Azure Portal에서 로그인한 다음 다시 로그인합니다. Azure AD 역할 또는 Azure 리소스 역할을 활성화하면 정품 인증 단계가 표시될 것입니다. 모든 단계가 완료되면 '사인아웃' 링크가 표시됩니다. 이 링크를 사용하여 로그인할 수 있습니다. 이렇게 하면 대부분의 경우 활성화 지연이 해결됩니다.
2. PIM에서 역할의 구성원으로 나열되어 있는지 확인해야 합니다.
3. 관리자 역할을 활성화하는 Exchange 로그인한 후 다시 로그인해야 합니다. 문제가 계속되면 지원 티켓을 열고 문제로 제기합니다. 관리자 역할을 사용하여 Exchange 및 준수 센터에 액세스하는 경우 다음 단계를 참조합니다.
4. 보안 및 준수 센터에 액세스하기 위해 역할을 활성화하거나 SharePoint 관리자 역할을 활성화하는 경우 몇 분에서 몇 시간까지 정품 인증이 지연됩니다. 이는 알려진 문제로, 이 문제를 최대한 빨리 해결하기 위해 이러한 팀과 적극적으로 협력하고 있습니다.

자세한 내용은 다음 항목을 참조하세요.

- [PIM에서 Azure AD 역할 활성화](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [PIM에서 Azure 리소스 역할 활성화](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**역할을 비활성화하거나 역할 활성화가 만료된 후 사용 권한이 제거되지 않습니다.**

Azure AD Privileged Identity Management 비활성화하거나 역할 활성화 기간이 만료되면 액세스 권한이 계속 지연될 수 있습니다.

비활성화가 지연되는 경우 다음 단계를 수행합니다.

1. Exchange 관리자 역할을 비활성화하거나 역할 활성화 기간이 만료되는 경우 사용 권한이 제거되기 전에 상당한 지연이 발견되면 지원 티켓을 열고 지원 엔지니어에게 이 문제와 관련한 Office PAM(Privileged Access Management) 팀에 티켓을 제출할 수 있도록 지원 엔지니어에게 요청하세요.
2. 정품 인증 기간이 만료된 경우 브라우저 세션이 열려 있는 경우 브라우저를 닫습니다. 해당 세션을 닫을 때까지 역할을 계속 사용할 수 있습니다. 이는 알려진 문제로, 정품 인증이 만료되면 각 세션을 적극적으로 해지하는 잠재적인 수정 방법을 찾고 있습니다.

지연이 이러한 두 시나리오와 다른 경우 지원 티켓을 열기 바랍니다.
