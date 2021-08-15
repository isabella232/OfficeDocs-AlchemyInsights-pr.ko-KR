---
title: 테넌트 삭제
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993899"
---
# <a name="delete-tenant"></a>테넌트 삭제

Azure AD를 삭제하려면 다음을 보장합니다.
- 디렉터리의 전역 관리자입니다.
- 로그인한 계정(예: contoso.onmicrosoft.com 계정)의 기본 디렉터리가 있는 계정으로 로그인하지 admin@contoso.onmicrosoft.com.
- 삭제하기 전에 디렉터리에서 활성 응용 프로그램을 제거합니다. 활성 응용 프로그램을 제거하려면 앱 등록으로 이동하여 기존 응용 프로그램을 제거합니다.
- 디렉터리에 연결된 Microsoft Online Services, Microsoft Azure, Office 365 Azure AD Premium 구독이 없습니다. Azure 지원 및 청구를 통해 구독을 이전하거나 활성 구독을 급히 취소합니다. 자세한 내용은 How to Cancel Office 365 and Azure subscriptions를하세요. 테넌트에 기존 구독을 연결하거나 추가하는 방법에 대한 지침은 Azure AD 테넌트에 Azure 구독 연결 또는 [추가를 참조하세요.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- 활성 라이선스가 없습니다. 라이선스를 제거하려면 [라이선스를 제거하는 구독을 제거하는 방법을 참조하세요.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- Azure AD를 삭제하려고 할 때 자신을 전역 관리자로 대신하여 디렉터리에 다른 활성 사용자가 없습니다. 다른 활성 사용자를 제거하고 테넌트의 사용자 지정 도메인 이름에 대한 종속성도 제거해야 합니다(예: 사용자 지정 도메인을 사용하여 만든 admin@contoso.com.

방법에 대한 자세한 단계는 다음을 참조하세요.
- "Azure Active Directory" 또는 "구독"을 삭제하려면 [Delete Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- 디렉터리에서 응용 프로그램을 제거하면 응용 프로그램 [제거를 참조합니다.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
