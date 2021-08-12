---
title: Intune 관리 콘솔 사용 시 발생하는 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 9310e8685a922207be8d5672d7929e19313cbb57e0fa6d25de149106692e811f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944137"
---
# <a name="problems-using-the-intune-admin-console"></a>Intune 관리 콘솔 사용 시 발생하는 문제

**Intune 관리 포털을 탐색하는 경우 "액세스 거부" 문제가 발생합니다.**

- 사용자가 Intune 사용자 지정 역할의 구성원이면 사용자의 계정에 Intune 또는 EMS(Enterprise Mobility Suite) 라이선스가 할당되어 있는지 확인합니다.
- 구성 관리자를 사용하여 장치를 관리하는 경우 구성 관리자 MDM의 Intune 사용자 모음에 속하지 않는지 확인합니다.
- Intune 역할 블레이드에서 해당 RBAC(역할 기반 관리 제어) 권한이 할당되었는지 확인합니다.
- 사용된 그룹이 메일 그룹이 아닌지 확인합니다. Azure 포털의 Intune에서는 Azure Active Directory 보안 그룹에 속한 사용자 계정만 지원합니다. Azure 포털 > **Intune** > **그룹** 또는 Azure 포털 **Azure Active Directory** 에서 그룹을 검토합니다.

**사용자에게 할당된 Intune 역할에 대한 사용 권한이 너무 많습니다.**

사용자는 **Intune** > **Intune 역할** > **내 사용 권한** > **내보내기** 로 이동하여 부여된 사용 권한을 검토하는 것이 좋습니다.

**역할에 범위 그룹을 추가했지만 해당 역할의 사용자가 다른 사용자 또는 장치를 계속 보게 됩니다.**

범위 그룹은 사용자나 장치를 필터링하지 않습니다. 범위 그룹:

- 사용자가 정책 또는 응용 프로그램을 할당할 수 있는 대상을 제한합니다.
- 특정 사용자만 장치에서 원격 작업을 실행할 수 있도록 허용합니다.

범위 그룹에 대한 자세한 내용은 [Microsoft Intune에서 RBAC(역할 기반 액세스 제어)](https://docs.microsoft.com/intune/role-based-access-control)를 참조하세요.

**Intune 역할에 사용자를 추가했지만 Intune 관리 콘솔에 대한 전체 액세스 권한을 계속 보유하고 있습니다.**

Azure 포털에서 Intune > **사용자** 로 이동하여 사용자가 Azure 포털에서 다음 역할 중 하나에 할당되어 있지 않은지 확인합니다.

- 전역 관리자
- Intune 서비스 관리자
- SharePoint 관리자

자세한 내용은 [Microsoft Intune에서 RBAC(역할 기반 액세스 제어)](https://docs.microsoft.com/intune/role-based-access-control)를 참조하세요.

**액세스 문제**

자세한 내용은 [Office 365, Azure 또는 Intune에 로그인할 수 없음](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)을 참조하세요.