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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806045"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD Connect 업그레이드

기본적으로 자동 업그레이드는 Azure AD Connect에서 사용 하도록 설정 되어 있으므로 최신 버전을 실행 하 고 있는지 확인할 수 있습니다. 자동 업그레이드 설정을 확인 하려면 Azure AD PowerShell에서 **ADSyncAutoUpgrade** cmdlet을 사용 합니다. Cmdlet은 다음 값 중 하나를 반환 합니다.

- **Enabled**: 자동 업그레이드가 사용 되도록 설정 됩니다.

- **사용 안**함: 자동 업그레이드가 사용 하지 않도록 설정 됩니다.

- **Suspended**: 시스템이 더 이상 자동 업그레이드를 받을 수 없습니다. 이 값은 구성할 수 없습니다. 시스템에서 설정 합니다.

자세한 내용은 [자동 업그레이드](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)를 참조 하세요.

최신 버전의 Azure AD Connect를 다운로드 하려면로 이동 [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) 합니다.
