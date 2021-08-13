---
title: 사용자 관리 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 70f8def2a0f3419a9aa6325e376ba52fc35ec48b61f39ede99d7e58cd6c6c464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971463"
---
# <a name="user-management-issues"></a>사용자 관리 문제

**'사용자 할당 필요' 속성을 사용하지 않도록 설정하면(이 속성을 아니요로 설정) 응용 프로그램에 현재 할당된 사용자가 어떻게 되나요?**

**사용자 할당 필요** 를 불가능으로 설정해도 현재 할당된 사용자는 영향을 받지 않습니다. 이 속성을 사용하지 않도록 설정하면 모든 사용자가 응용프로그램에 액세스할 수만 있습니다. 나열된 모든 사용자와 응용 프로그램에서 그룹에 할당된 사용자는 모두 유효합니다.

- 앱을 특정 사용자 집합으로 제한하는 경우 [Azure 애플리케이션을 사용자 집합으로 제한 - Microsoft ID 플랫폼 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)를 참조하세요.
- Azure Portal 내에서 또는 PowerShell을 사용하여 Azure AD의 엔터프라이즈 응용 프로그램에 사용자 및 그룹을 할당하려면 [Azure Active Directory의 앱에 대한 사용자 할당 관리](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)를 참조하세요.
- 응용 프로그램 만들기 및 관리 권한을 위임하려면 [응용 프로그램 관리 관리자 권한 위임 - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles)를 참조하세요.
- **사용자로부터 특정 엔터프라이즈 앱 숨기기** - 다음 단계에 따라 **MyApps** 패널에서 모든 Microsoft 365 앱을 숨깁니다. Office 365 포털에도 앱이 표시됩니다.

 1. 디렉터리의 전역 관리자로 Azure Portal에 로그인합니다. 
 2. **Azure Active Directory** 를 선택합니다. 
 3. **사용자** 를 선택합니다. 
 4. **사용자 설정** 을 선택합니다. 
 5. **엔터프라이즈 응용 프로그램** 에서 **최종 사용자 실행 및 응용 프로그램 보기 관리** 를 클릭합니다. 
 6. **Office 365 포털의 사용자만 Office 365 앱을 볼 수 있음** 에 대해 **예** 를 클릭합니다. 
 7. **저장** 을 클릭합니다. 
 8. 자세한 내용은 [Microsoft Azure AD의 사용자 환경에서 터프라이즈 응용 프로그램 숨기기 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)를 참조하세요.

- SaaS(Software as a Service) 앱을 여러 조직에 제공하는 경우 Azure AD(Azure Active Directory) 테넌트에서 로그인을 수락하도록 앱을 구성할 수 있습니다. 이 구성을 "응용 프로그램 다중 테넌트 만들기"라고 합니다. Azure AD 테넌트의 사용자는 앱에 계정을 사용하는 데 동의한 후 앱에 로그인할 수 있습니다. 자세한 내용은 [Azure AD 사용자에 로그인하는 앱 빌드 - Microsoft ID 플랫폼 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)를 참조하세요.

- **최종 사용자가 응용 프로그램에 할당된 후 응용 프로그램에 어떻게 액세스할 수 있나요?**

엔터프라이즈 응용 프로그램의 각 응용 프로그램에는 최종 사용자가 액세스할 수 있는 링크가 있습니다. 사용자는 **Myapps** 포털을 통해 앱에 쉽게 액세스할 수 있습니다.

- **사용자가 사용하려는 응용 프로그램과 응용 프로그램 유형을 알고 싶나요?**

**portal.azure.com > Azure Active directory> 로그인> 보고서 다운로드** 에서 지난 30일간의 로그인 보고서를 다운로드할 수 있습니다.

- [테넌트 전체 관리자에게 응용 프로그램에 대한 동의 허용](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) 및 [최종 사용자가 응용 프로그램에 동의하는 방식을 구성하는 방법](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)에 대해 알아봅니다.

- [동의 작동 방식](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 및 [응용 프로그램에 대한 동의 관리](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)를 이해합니다.


