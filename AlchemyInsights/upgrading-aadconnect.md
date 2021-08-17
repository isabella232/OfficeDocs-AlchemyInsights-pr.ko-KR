---
title: 932 AADConnect 업그레이드
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104818"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD 커넥트

기본적으로 Azure AD 커넥트 자동 업그레이드가 사용하도록 설정되어 최신 버전을 실행하는 데 도움이 됩니다. 자동 업그레이드 설정을 확인하려면 Azure AD PowerShell에서 **Get-ADSyncAutoUpgrade** cmdlet을 사용합니다. 이 cmdlet은 다음 값 중 하나를 반환합니다.

- **사용:** 자동 업그레이드가 사용하도록 설정됩니다.

- **사용 안 합니까:** 자동 업그레이드를 사용할 수 없습니다.

- **일시 중단:** 시스템이 더 이상 자동 업그레이드를 받을 수 없습니다. 이 값은 구성할 수 없습니다. 시스템에서 설정됩니다.

자세한 내용은 자동 [업그레이드를 참조하세요.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)

최신 버전의 Azure AD 앱을 다운로드하려면 커넥트 로 [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) 이동하세요.
