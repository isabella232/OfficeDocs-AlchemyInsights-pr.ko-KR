---
title: 백스캐터 공격으로부터 보호
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898022"
---
# <a name="protection-from-backscatter-attack"></a>백스캐터 공격으로부터 보호

백스캐터는 보내지 않은 메시지에 대해 수신하는 전달 실패 보고서(NDRS 또는 반송 메시지라고도 함)입니다. 스팸 발송자는 메시지의 **보낸 사람:** 주소를 위조(스푸핑)하며 메시지에 대한 신뢰성을 제공하기 위해 실제 전자 메일 주소를 사용하는 경우가 많습니다. 따라서 스팸 발송자가 불가피하게 존재하지 않는 수신자에게 메시지를 보낼 때 대상 전자 메일 서버는 기본적으로 NDR의 전달 불가능한 메시지를 **보낸 사람:** 주소의 위조된 보낸 사람에게 반환하도록 속입니다.

추가 정보는 [EOP의 백스캐터](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)에서 확인할 수 있습니다.

**백스캐터 보호 사용**

백스캐터 보호를 활성화하려면 아래 경로를 따르세요.

**protection.office.com > 위협 관리 > 정책 > 스팸 차단 정책 및 편집 > 스팸 속성 선택 > 스팸으로 표시 > NDR 백스캐터로 표시 > "켬"으로 설정**

계정이 손상되었다고 생각되는 경우 다음을 참조하세요.

- [손상된 전자 메일 계정에 응답](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Office 365의 제한된 사용자 포털에서 차단된 사용자 제거](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



