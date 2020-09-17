---
title: Intune을 사용한 조건부 액세스
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807665"
---
# <a name="conditional-access-with-intune"></a>Intune을 사용한 조건부 액세스

Intune을 사용 하 여  **조건부 액세스**  를 사용 하려면 3 단계가 필요 합니다.

- 장치가 호환 되는 것으로 간주 되기 전에 충족 해야 하는 설정을 정의 하는  **준수 정책**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows))을 만듭니다. 예를 들어 장치에는 호환 되는 것으로 간주 되기 전에 6 자리 이상의 pin이 있어야 합니다.
- 보호할 리소스와 해당 리소스에 액세스 하기 위해 충족 해야 하는 조건을 정의 하는 **조건부 액세스 정책을**  만듭니다.  [예를 들어](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  회사 전자 메일에 액세스 하기 전에 장치가 규격 이어야 합니다.
- **준수 정책과** **조건부 액세스 정책이** 모두 원하는 사용자 그룹을 대상으로 하는지 확인 합니다. 이를 위해서는 Azure Active Directory에서 특정 사용자 그룹을 만들어야 할 수 있습니다.

**유용한 링크:**

[장치 준수 개요](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA 문제 해결](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[문제 해결 정책](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

비규격 장치에서 전자 메일 (Exchange online)을 액세스 하지 못하도록 보호 하려면 두 문서를 모두 준수 해야 합니다.

1. [EAS를 사용 하 여 장치에서 전자 메일 액세스 보호](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Outlook과 같은 최신 인증 클라이언트를 사용 하 여 장치에서 전자 메일 액세스 보호](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)