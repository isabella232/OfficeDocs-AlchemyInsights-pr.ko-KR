---
title: 권한 있는 Id 관리 역할
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086379"
---
# <a name="privileged-identity-managementpim-role"></a>PIM (권한 Id 관리) 역할

**역할을 활성화 한 후에 권한이 부여 되지 않음**

Azure AD PIM (권한 부여 Id 관리)에서 역할을 활성화 하면 권한 있는 역할이 필요한 모든 포털에 인증이 즉시 전파 되지 않을 수 있습니다. 변경 내용이 전파 되더라도 포털의 웹 캐싱으로 인해 변경 내용이 즉시 적용 되지 않을 수 있습니다.

정품 인증이 지연 되는 경우 다음 단계를 수행 합니다.

1. Azure portal에서 로그 아웃 한 다음 다시 로그인 하세요. Azure AD 역할 또는 Azure 리소스 역할을 활성화 하면 정품 인증 단계가 표시 됩니다. 모든 단계가 완료 되 면 ' 로그 아웃 ' 링크가 표시 됩니다. 이 링크를 사용 하 여 로그 아웃할 수 있습니다. 이렇게 하면 대부분의 경우 정품 인증 지연에 대 한 해결이 실행 됩니다.
2. PIM에서 역할의 구성원으로 나열 되어 있는지 확인 합니다.
3. Exchange 관리자 역할을 활성화 하는 경우 로그 아웃 하 고 다시 로그인 해야 합니다. 문제가 계속 되 면 지원 티켓을 열고 문제를 제기 합니다. Exchange 관리자 역할을 사용 하 여 보안 및 준수 센터에 액세스 하는 경우 다음 단계를 참조 하세요.
4. 보안 및 준수 센터에 액세스 하기 위해 역할을 활성화 하거나 SharePoint 관리자 역할을 활성화 하는 경우 몇 분에서 몇 시간까지 몇 가지 정품 인증 지연이 발생 합니다. 이는 알려진 문제 이므로 가능한 한 빨리이 문제를 해결 하기 위해 이러한 팀과 협력 하 고 있습니다.

자세한 내용은 다음을 참조하시기 바랍니다.

- [PIM에서 내 Azure AD 역할 활성화](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [PIM에서 내 Azure 리소스 역할 활성화](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**역할을 비활성화 하거나 역할 활성화가 만료 된 후에 사용 권한이 제거 되지 않음**

Azure AD 권한 있는 Id 관리에서 역할을 비활성화 하거나 역할 활성화 기간이 만료 되는 경우 계속 해 서 액세스 권한이 있을 수 있습니다.

비활성화가 지연 되는 경우 다음 단계를 수행 합니다.

1. Exchange 관리자 역할을 비활성화 하거나 역할 활성화 기간이 만료 되는 경우 사용 권한이 제거 되기 전에 상당한 지연이 발생 하면 지원 티켓을 열고 지원 엔지니어에 게 문의 하 여이 문제에 대해 Office 내부의 PAM (권한 부여 관리) 팀과 티켓을 파일 하는 데 도움을 주어 야 합니다.
2. 정품 인증 기간이 만료 되었지만 여전히 브라우저 세션이 열려 있으면 브라우저를 닫습니다. 해당 세션을 닫을 때까지이 역할을 계속 사용할 수 있습니다. 이는 알려진 문제로, 정품 인증이 만료 된 후에 각 세션을 적극적으로 해지 하기 위해 가능한 수정 사항을 확인 하 고 있습니다.

지연 시간이 이러한 두 시나리오와 다를 경우 지원 티켓을 여십시오.
