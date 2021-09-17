---
title: Microsoft Teams 조직 차트에 여전히 사용자 사진이 표시됨
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2021
ms.locfileid: "59334382"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Microsoft Teams 조직 차트에 여전히 사용자 사진이 표시됨

조직의 개인 한 명 이상이 비활성화되거나 제거된 경우 조직 차트에 프로필 사진이 여전히 표시된다면 **ShowInAddressLists** 설정이 False로 설정되어 있을 수 있습니다. 

1. Microsoft 365 관리 센터 > [활성 사용자](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)로 가서 계속 사진이 표시되는 사용자를 선택합니다. 
1. **메일** 탭을 선택한 다음 **전체 주소 목록에서 표시** 를 **안 함** 으로 설정합니다.

**ShowInAddressLists** 를 **안 함** 으로 설정해도 문제가 해결되지 않는다면 다음을 확인합니다. 

- Exchange의 받는 사람 목록에 사용자가 숨겨져 있을 수 있습니다. 자세한 내용은 [Exchange Online의 주소 목록 관리](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists)를 참조하세요. 
- Azure Active Directory의 주소 목록에 사용자가 표시될 수 있습니다. 자세한 내용은 [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0)를 참조하세요. 