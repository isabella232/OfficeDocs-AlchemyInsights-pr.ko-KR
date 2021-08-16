---
title: 여러 개체의 전자 메일 주소가 ID와 동일합니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 5866d182cb2e97e37bc6df87e05fb6ef55bfed1d36f9daa95b7b8993a509e2dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011918"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>여러 개체의 전자 메일 주소가 ID와 동일합니다.

**여러 개체**

이 오류가 발생하는 일반적인 이유 중 하나는 전자 메일 주소가 ID와 동일한 여러 개체가 존재하여 Outlook Web Access 요청을 올바르게 라우팅할 수 없기 때문입니다. 이러한 개체를 찾으려면 다음 명령을 실행합니다.

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

이 문제를 해결하려면 동일한 전자 메일 ID가 있는 여러 개체를 제거하고 특정 전자 메일 ID가 포함된 단일 개체가 있고 해당하는 받는 사람 형식이 UserMailbox인지 확인합니다.

**동일한 주소가 비즈니스 및 소비자 사서함에 사용됩니다.**

또 다른 원인은 동일한 주소를 비즈니스 및 소비자 사서함에 사용하는 경우입니다. 이 경우, 카페에서 이 시나리오를 지원할 때까지는 사용자가 기본 소비자 별칭을 변경해야 합니다. 이는 개입 없이는 사라지지 않는 영구적인 오류입니다.

자세한 내용은 [Microsoft 계정의 전자 메일 주소 또는 전화 번호 변경](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)을 참조하세요.