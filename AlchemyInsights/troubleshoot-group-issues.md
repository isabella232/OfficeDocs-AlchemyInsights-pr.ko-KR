---
title: 그룹 문제 해결
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 47f00118a5a4b446b6a3b06f0fc6101d00d11b626eaf249bb6ca962a55f7f4d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939349"
---
# <a name="troubleshoot-group-issues"></a>그룹 문제 해결

**Azure AD 역할에 그룹을 할당해야 하는 경우**

Azure AD 역할에 Azure AD(Active Directory) 그룹을 할당하는 경우 다음 단계를 수행합니다.

1. 새 그룹 만들기-새 그룹을 만들려면 :

    a. 권한 있는 역할 관리자 또는 전역 관리자 권한으로 Azure AD 관리 센터에 로그인합니다. 
    b. Azure Active Directory> 그룹> 모든 그룹> 새 그룹을 선택합니다. 
    c. 그룹을 만듭니다.

2. 그룹을 만드는 동안 또는 그룹을 만든 후에 역할을 그룹에 할당합니다.

    a. 그룹 생성시 그룹에 역할을 할당하려면 Azure AD 역할을 그룹에 할당할 수 있음 토글을 켜고 그룹을 만듭니다.
    b. 그룹을 만든 후 그룹에 역할을 할당하려면 새로 만든 그룹의 할당된 역할 탭으로 이동하여 그룹에 역할을 할당합니다.

**Azure AD 역할에 할당된 그룹의 구성원 자격을 관리해야 하는 경우**

1. 권한 상승을 방지하기 위해 기본적으로 권한 있는 역할 관리자와 전역 관리자만 역할에 할당된 그룹의 구성원 자격을 수정할 수 있습니다. 그러나 이러한 그룹에 대한 소유자를 지정하고 이 작업을 대리하도록 선택할 수 있습니다. 자세한 내용은 [Azure Active Directory에서 클라우드 그룹을 사용하여 역할 할당](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)을 참조하세요.
2. Azure AD의 그룹에 역할을 할당하기 위한 일반적인 질문과 문제 해결 팁은 [클라우드 그룹에 할당된 역할 문제 해결](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)을 참조하세요.

**동적 그룹**

1. 기본 제공 사용자 특성을 찾을 수 없는 경우 이 특성이 지원되는 속성 목록에 나열되어야 합니다.
2. 기본 제공 장치 특성을 찾고 있는 경우 특성이 장치 특성 목록에 표시되어야 합니다. 
3. 기본 제공 사용자 및 장치 특성 외에도 [확장 특성](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties)도 사용할 수 있습니다. 확장 특성을 온-프레미스 Windows Server AD 또는 연결된 SaaS 응용 프로그램에서 동기화하면 규칙 작성기 드롭다운 목록에 특성이 표시됩니다. PowerShell을 사용하여 사용자 특성을 쿼리하고 특성 이름을 검색하여 사용자 지정 특성 이름을 디렉터리에서 찾을 수 있습니다. 규칙 구문에서 규칙을 구성할 때도 이러한 규칙을 사용할 수 있습니다.
4. 테넌트에 적절한 라이선스가 부여되었는지 확인합니다. 동적 그룹을 사용하려면 테넌트에 Azure AD P1 Premium 라이선스가 필요합니다. [여기](https://azure.microsoft.com/pricing/details/active-directory/)에서 Azure AD 라이선스 계획 목록에 액세스할 수 있습니다. Enterprise Mobility + Security 라이선스 계획은 [여기](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)에서 액세스할 수 있습니다.
5. 동적 그룹을 만드는 사용자의 역할이 전역 관리자, intune 관리자, 그룹 관리자 또는 사용자 관리자인지 합니다.
6. 그룹이 채워지도록 시간을 허용하세요. 그룹은 테넌트의 크기에 따라 처음 또는 규칙 변경 후 채우는 데 최대 24시간이 걸릴 수 있습니다.
7. 자세한 내용은 [그룹 구성원 자격에 대한 특성 기반 규칙 만들기](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)를 참조하세요.

**그룹을 삭제해야 하는 경우**

1. Azure AD PowerShell 모듈의 Remove-AzureADGroup cmdlet을 사용하여 디렉터리에서 그룹을 삭제할 수 있습니다.
2. Azure AD에서 동기화된 그룹을 삭제하기 전에 먼저 오류 발생을 방지하기 위해 할당된 모든 라이선스를 삭제했는지 확인합니다.
3. 그룹 삭제에 대한 자세한 내용은 [할당된 라이선스가 할당된 그룹 삭제](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)를 참조하세요.

**삭제된 그룹을 복원해야 하는 경우**

1. Office 365 그룹이 삭제된 경우 영구 삭제가 발생하기 최대 30일 전까지만 복원할 수 있습니다. 영구적으로 삭제된 그룹은 더 이상 복원할 수 없습니다. [여기](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)에서 그룹 복원에 대해 자세히 알아보세요.
2. 이 기능은 보안 그룹 및 메일 그룹에서 지원되지 않습니다.
3. Office 365 그룹을 복원할 수 있는 권한이 있는지 확인합니다. 전역 관리자, 그룹 관리자, 사용자 계정 관리자, intune 서비스 관리자, 파트너 티어 1 또는 티어 2 지원 및 그룹 소유자는 그룹을 복원할 수 있습니다.
4. 동적 그룹이 삭제 및 복원되면 해당 그룹이 새 그룹으로 표시되고 규칙에 따라 다시 채워집니다. 이 프로세스는 최대 24시간이 걸릴 수 있습니다.
5. 삭제된 그룹 복원에 대한 자세한 내용은 [Azure Active Directory에서 삭제된 Office 365 그룹 복원](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)을 참조하세요.

**그룹 만료 정책 구성**

1. 이 기능은 Office 365 그룹에만 지원될 뿐, 보안 그룹 및 메일 그룹에는 지원되지 않습니다.
2. Office 365 그룹의 만료 정책을 구성하고 사용하려면 Azure AD Premium 라이선스가 필요합니다.
3. 현재 테넌트의 Office 365 그룹에 대해 하나의 만료 정책만 구성할 수 있습니다.
4. 전역 관리자, 그룹 관리자, 사용자 관리자 및 그룹의 소유자만 그룹을 갱신할 수 있습니다.
5. Office 365 그룹이 만료된 경우, 해당 그룹은 삭제되며 영구 삭제가 발생하기 최대 30일 전까지만 복원할 수 있습니다. 영구적으로 삭제된 그룹은 더 이상 복원할 수 없습니다. [여기](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)에서 그룹 복원에 대해 자세히 알아보세요.

**활동 기반 자동 갱신**

SharePoint, Outlook 및 Teams의 사용자 활동은 그룹 자동 갱신을 트리거할 수 있습니다. 활동은 그룹이 만료되기 35일 전에 검사됩니다. 현재 그룹 수명 주기 동안 활동이 있는 경우 그룹이 자동으로 갱신되고 그룹 소유자에게 전자 메일 알림이 전송되지 않습니다.

**만료된 그룹의 알림 타이밍**

1. 전자 메일 알림은 그룹 만료 30일, 15일 및 1일 전에 Office 365 그룹 소유자에게 전송됩니다.
2. 처음 만료를 설정할 때 만료 간격보다 오래된 그룹은 만료까지 35일로 설정됩니다.
3. 그룹 만료 날짜는 정책 업데이트 날짜가 아니라 그룹의 갱신 날짜를 기준으로 계산됩니다. 만료 정책이 업데이트되는 경우 만료 날짜는 변경되지 않습니다.
4. 자세한 내용은 [그룹 만료 정책 및 갱신 전자 메일](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) 및 [Azure Active Directory 365에서 삭제된 Office 365 그룹 복원](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)을 참조하세요.

**그룹을 만들 수 있는 권한**

새 그룹을 만들 수 있는 권한을 부여받았는지 확인합니다. 전역 관리자는 Azure 포털 또는 액세스 패널에서 그룹 만들기를 사용하지 않도록 설정할 수 있습니다. 관리자가 새 그룹을 만들거나 적절한 사용 권한을 부여해야 할 수 있습니다.

1. [Azure Portal에서 새 그룹 만들기 및 구성원 추가](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [PowerShell MSOnline에서 그룹 만들기](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [PowerShell에서 그룹 만들기 사용 해제](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Office 365에서 그룹을 만들 수 있는 사용자 관리](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Powershell을 통해 Office 365 시작 알림 사용 해제](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Azure AD 관리 역할](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**그룹 만들기 권한 관리**

1. 전역 관리자는 **사용자가 Azure Portal에서 보안 그룹을 만들 수 있음** 또는 **사용자가 **모든 그룹> 일반(설정)** 의 Azure Portal 설정에서 Office 365 그룹을 만들 수 있음** 을 설정하여 Azure Portal 또는 액세스 패널에서 만든 보안 또는 Office 365 그룹에 대한 그룹 만들기 권한을 관리할 수 있습니다.
2. Azure AD P1 Premium 라이선스가 있는 경우 그룹 만들기를 제한하여 사용자 그룹을 선택할 수 있습니다.

**Office 365 그룹의 새 구성원에 대해 시작 알림 사용 해제**

Office 365 그룹에 추가된 사용자에게 전송되는 환영 알림은 Powershell에서 `UnifiedGroupWelcomeMessageEnabled`을(를) **거짓** 으로 설정하여 사용 해제할 수 있습니다. [여기](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)에서 이 설정에 대해 자세히 알아보세요.













