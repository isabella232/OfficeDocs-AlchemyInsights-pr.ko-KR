---
title: 646 AADConnect를 구성하는 방법
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
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963649"
---
# <a name="configure-sync-features"></a>동기화 기능 구성

Azure AD 커넥트 기본적으로 사용하도록 설정되거나 나중에 사용하도록 설정할 수 있는 여러 기능이 포함되어 있습니다. 일부 기능을 사용하려면 특정 환경에서 추가 구성이 필요합니다.

- [필터링은](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) 개체가 Azure AD에 동기화되는 제한입니다. 기본적으로 모든 사용자, 연락처, 그룹 및 Windows 10 계정이 동기화됩니다. 도메인, US 또는 기타 특성에 따라 개체를 포함하거나 제외할 수 있습니다.

- [암호 해시 동기화는](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) 암호 해시를 Azure AD에 동기화합니다. 이렇게 하면 한 위치에서 암호를 관리하지만, 사내 및 클라우드 환경에서 동일한 암호를 사용할 수 있습니다. Active Directory는 권한이 있는 원본이기 때문에 자체 암호 정책을 사용할 수 있습니다.

- [SSPR(셀프](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) 서비스 암호 재설정)을 사용하면 사용자가 클라우드에서 자신의 암호를 다시 설정하는 동시에, 여전히 프레미스 암호 정책을 적용할 수 있습니다.

- [장치 쓰기](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) 저장소를 사용하면 조건부 액세스에 사용할 수 있도록 Azure AD의 등록된 장치를 다시 프레미스 Active Directory에 기록할 수 있습니다.

- [실수로 인한](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) 삭제 방지는 기본적으로 너무 많은 동시 개체 삭제(동기화당 개체 500개 이상)를 방지하는 데 사용됩니다. 조직의 요구에 따라 이 설정을 변경할 수 있습니다.

- [자동 업그레이드는](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) 기본적으로 익스프레스 설치에 대해 사용하도록 설정되어 있으며 Azure AD 응용 커넥트 항상 최신 버전이 되도록 합니다.
