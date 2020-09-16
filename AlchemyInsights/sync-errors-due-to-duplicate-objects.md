---
title: 902 (중복 된 개체로 인 한 동기화 오류)
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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737347"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>개체가 중복 되어 동기화 오류가 발생 했습니다.

Microsoft 365에서 디렉터리 동기화가 완료 되 면 다음과 같은 오류 메시지 중 하나가 나타날 수 있습니다.

- 이 개체와 연결 된 다음 특성은 로컬 디렉터리의 다른 개체와 이미 연결 되어 있을 수 있는 값을 가지 므로 Microsoft Online Services에서이 개체를 업데이트할 수 없습니다.

- 프록시 주소가 같은 synchronized 개체가 Microsoft Online Services 디렉터리에 이미 있습니다.

- 이 개체와 연결 된 다음 특성에 로컬 디렉터리 서비스의 다른 개체와 이미 연결 되어 있을 수 있는 값이 있기 때문에이 개체를 업데이트할 수 없습니다. UserPrincipalName.

이 문제를 확인 하 고 해결 하려면 [Idfix DirSync 오류 수정 도구](https://www.microsoft.com/download/details.aspx?id=36832)를 다운로드 하 여 실행 합니다.

자세한 내용은 [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)를 참조 하십시오.
