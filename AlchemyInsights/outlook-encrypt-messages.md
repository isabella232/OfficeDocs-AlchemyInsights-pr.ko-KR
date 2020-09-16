---
title: 웹용 Outlook의 S/MIME
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772304"
---
# <a name="encrypt-email-messages-in-outlook"></a>Outlook에서 전자 메일 메시지 암호화

Microsoft 365 메시지 암호화는 Azure Information Protection의 일부인 Azure RMS (Microsoft Azure Rights Management)를 기반으로 합니다. Azure 권한 관리 또는 Azure Information Protection이 구독에 포함 되어 있는 경우에는 권한 관리 서비스를 **수동으로 사용 하거나 활성화 하기 위해 작업을 수행할 필요가 없습니다** .

고객 의견에 따라 더 이상 Exchange 메일 흐름 규칙을 사용 하 여 테 넌 트에 특정 유형의 중요 한 정보를 포함 하는 아웃 바운드 전자 메일을 기본적으로 자동 암호화 하지 않습니다. 대신이 yourselves를 수행 하는 방법에 대 한 자세한 지침을 제공 합니다. 중요 한 정보를 암호화 하는 전송 규칙을 만드는 방법에 대 한 자세한 내용은 [이 문서](https://aka.ms/OmeEtr)를 참조 하십시오.

- 웹용 Outlook (이전에는 **owa**)을 사용 하는 경우 전자 메일 메시지를 작성할 때 Owa에서 **보호** 를 클릭 하면 됩니다. 이렇게 하면 "전달 금지" 권한이 적용 됩니다. **사용 권한 변경을** 클릭 하 고 **암호화** 를 선택 하 여 메시지만 암호화 합니다.

- **Outlook 클라이언트**를 사용 하는 경우: outlook 2013 또는 2016 또는 Mac 용 outlook 2016에서 암호화 된 메시지를 보내려면 **옵션**  >  **사용 권한을**선택 하 고 필요한 보호 옵션을 선택 합니다.

- 특정 받는 사람이 나 외부 파트너 조직에 보낸 **모든 전자 메일을 자동으로 암호화** 하려면 Exchange 관리 센터에서 메일 흐름 전송 규칙을 만들어야 합니다. 자세한 지침은 [이 지원 문서](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)에 나와 있습니다.

