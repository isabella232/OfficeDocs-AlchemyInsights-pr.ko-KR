---
title: 902(중복 개체로 인한 동기화 오류)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998800"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>중복 개체로 인한 동기화 오류

디렉터리 동기화가 완료될 때 다음 오류 메시지 중 Microsoft 365.

- 이 개체와 연결된 다음 Microsoft Online Services 로컬 디렉터리의 다른 개체와 이미 연결되어 있을 수 있는 값이 있기 때문에 이 개체는 업데이트할 수 없습니다.

- 프록시 주소가 같은 동기화된 개체가 Microsoft Online Services 있습니다.

- 이 개체와 연결된 다음 특성에는 로컬 디렉터리 서비스의 다른 개체와 이미 연결되어 있을 수 있는 값이 있기 때문에 이 개체를 업데이트할 수 없습니다. UserPrincipalName.

문제를 식별하고 해결하려면 [IdFix DirSync](https://github.com/Microsoft/idfix)오류 수정 도구를 다운로드하여 실행합니다.

자세한 내용은 [KB2647098을 참조하세요.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
