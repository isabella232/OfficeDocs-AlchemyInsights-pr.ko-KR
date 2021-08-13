---
title: 공유 사서함을 만드는 동안 프록시 주소 오류
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062914"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>사서함 또는 다른 전자 메일 사용 개체를 만드는 동안 프록시 주소 오류

전자 메일 사용이 가능한 개체(사서함, 공유 사서함 등)를 만들려고 하여 "프록시 주소 "SMTP:alias@domain.com"가 이미 사용 중입니다."라는 오류가 표시되면 선택한 전자 메일 주소가 이미 조직의 다른 전자 메일 사용 개체에 의해 이동된 것입니다.
  
이 전자 메일 주소가 있는 사용자, 그룹, 공유 사서함 또는 공용 폴더를 찾아 삭제하거나 전자 메일 주소를 변경해야 합니다. 그런 다음 사용 가능한 전자 메일 주소가 있는 새 전자 메일 사용 가능 개체를 만들 수 있습니다. 홈 페이지에서 검색을 사용하여 검색합니다. PowerShell 명령에 다음 Exchange Online 사용하여 검색할 수도 있습니다.

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
기존 전자 메일 주소를 삭제하지 않는 경우 만들 새 개체의 새 전자 메일 주소를 선택하십시오.
  