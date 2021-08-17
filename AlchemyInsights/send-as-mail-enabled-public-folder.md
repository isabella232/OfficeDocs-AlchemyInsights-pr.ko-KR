---
title: EXO에서 메일 사용이 가능한 공용 폴더로 보내기
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
- "1956"
- "3500007"
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052572"
---
# <a name="sendas-mail-enabled-public-folder"></a>SendAs 메일 사용 가능 공용 폴더

다음 예에서는 메일 사용이 가능한 공용 폴더 NewPF1에 대해 "다른 사람으로 보내기" 권한을 사용자 Jason에게 할당합니다.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'

구문과 매개 변수에 대한 자세한 내용은 메일 사용이 가능한 공용 폴더에 대해 "다른 사람으로 보내기" 또는 "대신 보내기" 권한 [할당을 참조하십시오.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)

