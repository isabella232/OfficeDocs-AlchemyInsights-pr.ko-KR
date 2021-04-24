---
title: Exchange 관리 센터의 보존 정책이 작동하지 않습니다.
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952234"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange 관리 센터의 보존 정책

아래에 언급된 설정에 대한 자동 검사를 실행하려면 이 페이지 맨 위에 있는 뒤로 단추<-를 선택한 다음 보존 정책에 문제가 있는 사용자의 전자 메일 주소를 입력합니다.

Exchange 관리 센터의 보존 정책에 문제가 있는 경우 사서함이나 보관 사서함으로 이동하지 않는 항목에 적용하지 않는 경우 다음을 검사합니다.

**근본 원인:**

- **관리되는 폴더 도우미가** 사용자의 사서함을 처리하지 않았습니다. 관리되는 폴더 도우미는 7일마다 한 번씩 클라우드 기반 조직의 모든 사서함을 처리합니다.

  **해결 방법:** 관리되는 폴더 도우미를 실행합니다.

- **RetentionHold가** **사서함에서** 사용하도록 설정되어 있습니다. 사서함이 RetentionHold에 배치된 경우 해당 시간 동안 사서함의 보존 정책이 처리되지 않습니다.

  **해결 방법:** 보존 보류 설정의 상태를 확인하고 필요한 경우 업데이트합니다. 자세한 내용은 [Mailbox Retention Hold를 참조합니다.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**참고:** 사서함이 10MB보다 작은 경우 관리되는 폴더 도우미는 사서함을 자동으로 처리하지 않습니다.
 
Exchange 관리 센터의 보존 정책에 대한 자세한 내용은 다음을 참조하세요.

- [보존 태그 및 보존 정책](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [사서함에 보존 정책 적용](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) 또는 보존 태그 추가 [또는 제거](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [사서함의 보류 유형을 식별하는 방법](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
