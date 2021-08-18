---
title: 관리자를 추가 및 관리하는 방법 - 권장 단계
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 48a06fde215e007b6b81b32ab751ca8e4bba522d
ms.sourcegitcommit: 46e24d65cffd37b6988447c6738b3315303bbe13
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58339038"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>관리자를 추가 및 관리하는 방법 - 권장 단계

문제 설명에 따라 해결 방법을 찾을 수 있습니다. 대부분의 고객은 설명서를 따라 자신의 문제를 직접 해결할 수 있습니다.

**구독 관리자 또는 공동 관리자 편집**

- 계정 관리자는 두 역할을 모두 편집할 수 있는 반면 구독 관리자는 Azure Portal에서 공동 관리자만 변경할 [수 있습니다.](https://ms.portal.azure.com/#home)
- [Azure 구독 관리자 추가 또는 변경](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**내부(AIRS) Co-Administrator 구독 관리자 또는 구독 업데이트**

서비스 관리자 또는 공동 관리자는 다음 단계를 수행하여 이 작업을 자체적으로 서비스할 수 있습니다.

1. [Azure Portal에 로그인하고](https://ms.portal.azure.com/#home) 왼쪽 블레이드에서 비용 관리 **+** 청구를 클릭합니다.
2. 구독이 있는 품목을 클릭합니다. 그러면 구독에 대한 개요가 열립니다.
3. 구독 **블레이드에서** 속성을 **클릭합니다.** 
4. 서비스 **관리자 단추를** 클릭합니다.
5. 서비스 관리자로 설정할 사용자의 전자 메일을 입력하고 확인 을 **클릭합니다.**

**공동 관리자 추가/변경/제거**

1. [Azure Portal에 서비스](https://ms.portal.azure.com/#home) 관리자로 로그인합니다.
2. 구독을 [열고](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 구독을 선택합니다. 공동 관리자에게는 구독 범위에서만 할당할 수 있습니다.
3. **IAM(액세스 제어)** 클래식 관리자 추가 공동 관리자 추가로 이동하여 공동 관리자 추가 창을 열 수 있습니다(공동 관리자 추가 옵션을 사용하지 않도록 설정하면 권한이 없다는  >    >    >   것입니다). 
4. 추가할 사용자를 선택하고 추가 를 **클릭합니다.**

**자세한 정보:**
- [공동 관리자 추가](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [공동 관리자 제거](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [서비스 관리자 변경](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [계정 관리자 보기](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [RBAC 및 Azure Portal을 사용하여 액세스 관리](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**AD(사용자 추가/삭제) Azure Active Directory 추가/삭제**

Azure AD(Azure AD) 조직에서 새 사용자를 추가하거나 기존 사용자를 Azure Active Directory 수 있습니다.

1. 새 사용자를 추가하려면 [Azure Portal에](https://ms.portal.azure.com/#home) 조직의 사용자 관리자로 로그인합니다.
2. 를 **Azure Active Directory** 사용자를 **선택한** 다음 새 **사용자를 클릭합니다.**
3. 사용자 **페이지에서** 필요한 정보를 입력합니다. **만들기** 를 클릭합니다. 사용자가 만들어지며 Azure AD 테넌트에 추가됩니다.

**자세한 내용은 다음을(를) 자세히 알아보아**

- [새 사용자 추가](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [사용자 삭제](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [사용자 프로필 정보를 사용하여 사용자 프로필 정보 추가 또는 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**추천 문서**

- [RBAC(역할 기반 액세스 제어)란?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Azure의 다양한 역할 이해](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Azure Active Directory의 관리자 역할 권한](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [자습서: RBAC 및 Azure Portal을 사용하여 사용자에게 액세스 권한 부여](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Azure에서 RBAC 문제 해결](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Azure 관리 그룹을 사용하여 리소스 구성](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [전자 메일을 통해 Azure 송장 복사본을 요청하는 방법](https://azure.microsoft.com/blog/azure-email-invoices/)
- [Azure에서 신용 카드 또는 직불 카드를 추가, 업데이트 또는 제거하는 방법](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [구독 관리(다시 활성화/취소/전환)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



