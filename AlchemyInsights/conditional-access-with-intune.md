---
title: Intune을 통해 조건부 액세스
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069718"
---
# <a name="conditional-access-with-intune"></a>Intune을 통해 조건부 액세스

Intune에서  **조건부**  액세스를 사용하려면 다음 3단계가 필요합니다.

- 준수  [정책(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios) [, Windows )을](https://docs.microsoft.com//intune/compliance-policy-create-windows)만들어 장치가 규격으로 간주되기 전에 충족해야 하는 설정을 정의합니다. 예를 들어 장치에는 규정 준수로 간주되기 전에 최소 6자리의 핀이 있어야 합니다.
- 보호되는 리소스와 해당 **리소스에 액세스하기**  위해 충족해야 하는 조건을 정의하는 조건부 액세스 정책을 만들 수 있습니다.  [예를 들어 회사](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  전자 메일에 액세스하기 전에 장치를 준수해야 합니다.
- 준수 **정책과**  **조건부 액세스**  정책이 모두 원하는 사용자 그룹을 대상으로 하는지 확인 이 경우 사용자 그룹에 특정 사용자 그룹을 만들어야 Azure Active Directory.

**유용한 링크:**

[장치 준수 개요](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA 문제 해결](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[문제 해결 정책](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

전자 메일(Exchange)을 비호정 장치의 액세스로부터 보호하려면 두 문서를 모두 따라야 합니다.

1. [EAS를 사용하여 장치에서 전자 메일 액세스 보호](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [모바일 장치와 같은 최신 인증 클라이언트를 사용하여 장치에서 전자 메일 Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)