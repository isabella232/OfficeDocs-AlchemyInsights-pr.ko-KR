---
title: 응용 프로그램 삭제 또는 복원
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013985"
---
# <a name="delete-or-restore-applications"></a>응용 프로그램 삭제 또는 복원

**Azure AD 테넌트에서 응용 프로그램을 삭제하려면**

1. Azure **AD 포털에서** 엔터프라이즈 응용 **프로그램을 선택합니다.** 그런 다음 삭제할 응용 프로그램을 찾아 선택합니다.
2. 왼쪽 **창의** 관리 섹션에서 속성을 **선택합니다.**
3. **삭제를** 선택한 다음 **예를** 선택하여 Azure AD 테넌트에서 앱을 삭제하려는지 확인할 수 있습니다.

앱을 삭제하는 방법에 대한 자세한 내용은 [빠른 시작: Azure AD(Azure Active Directory)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)테넌트에서 응용 프로그램 삭제를 참조하세요.

PowerShell에서 [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet은 Azure Active Directory의 특정 응용 프로그램에서 응용 프로그램 프록시 구성을 제거하고 지정된 경우 응용 프로그램을 완전히 삭제할 수 있습니다.

PowerShell을 **사용하여 삭제된 응용** 프로그램을 복원할 수 있습니다. 복원할 응용 프로그램이 식별되면 [Restore-AzureADDeletedApplication을](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)사용하여 복원할 수 있습니다.
