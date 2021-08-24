---
title: Microsoft Teams 조직도에 사용자 사진이 표시되지 않음
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/23/2021
ms.locfileid: "58467379"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Microsoft Teams 조직도에 사용자 사진이 표시되지 않음

조직에서 한 명 이상의 개인 프로필 사진이 조직도에서 누락된 경우 **ShowInAddressLists** 를 **False** 로 설정한 것일 수 있습니다.

1. Microsoft 365 관리 센터 > [**활성 사용자**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)로 이동하여 사진이 누락된 사용자를 선택합니다. 
1. **메일** 탭을 선택하고 **전체 주소 목록에 표시** 가 **예** 로 설정되어 있는지 확인합니다. 

**ShowInAddressLists** 를 **예** 로 설정해도 작동하지 않으면 다음을 확인하세요.

- Exchange의 받는 사람 목록에 사용자가 숨겨져 있을 수 있습니다. 자세한 내용은 [Exchange Online의 주소 목록 관리](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists)를 참조하세요. 
- Azure Active Directory의 주소 목록에 사용자가 숨겨져 있을 수 있습니다.. 자세한 내용은 [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0)를 참조하세요. 
