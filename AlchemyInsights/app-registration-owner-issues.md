---
title: 앱 등록 소유자 문제
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123194"
---
# <a name="app-registration-owner-issues"></a>앱 등록 소유자 문제

다음은 앱 등록에 대한 소유자로 보안 주체를 추가하는 데 사용할 수 있는 방법입니다.

- Azure AD PowerShell 모듈 사용 -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    참조: [Add-AzureADApplicationOwner(AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Azure CLI 사용 - `az ad app owner add`

    참조: [az 광고 앱 소유자](https://docs.microsoft.com/cli/azure/ad/app/owner)
- MS Graph 사용 -

    참조: [소유자 추가 - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Azure AD 포털 사용 - Azure Active directory portal.azure.com [>](https://portal.azure.com/) Azure Active directory > 등록으로 > 응용 프로그램 선택> 소유자 > 추가

**해당 응용 프로그램의 소유자이어도 앱 등록 블레이드에서 응용 프로그램을 볼 수 없는 경우**

앱의 소유자는 관리 역할이 아니기도 합니다. [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) 관리 포털에 대한 액세스 제한 설정이 사용하도록 설정된 경우 관리자만 앱 등록 포털에서 응용 프로그램을 볼 수 있습니다. 소유자가 응용 프로그램을 볼 수 있도록 설정하려면 이 설정을 사용하지 않도록 설정하거나(이 설정을 NO로 설정) 특정 응용 프로그램에 대한 소유자에게만 관리자 역할을 할당합니다. 그러나 이를 위해 Azure AD Premium P2 라이선스가 필요하며 [Privileged Identity Management를 사용하도록 설정해야 합니다.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
