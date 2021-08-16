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
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010730"
---
# <a name="encrypt-email-messages-in-outlook"></a>전자 메일 메시지 암호화 Outlook

Microsoft 365 메시지 암호화는 Azure Microsoft Azure 보호의 일부인 Azure RMS(권한 관리)를 사용하여 구축됩니다. 구독에 Azure 권한 관리 또는 Azure  Information Protection이 포함된 경우 권한 관리 서비스를 수동으로 활성화하거나 활성화하기 위한 작업을 수행할 필요가 없습니다.

고객 의견에 따라 더 이상 Exchange 메일 흐름 규칙이 기본적으로 테넌트에 특정 유형의 중요한 정보가 포함된 아웃바운드 전자 메일을 자동으로 암호화할 수 없습니다. 대신, 이러한 작업을 어떻게 할 수 있는가에 대한 자세한 지침을 제공합니다. 중요한 정보를 암호화하는 전송 규칙을 만드는 방법에 대한 자세한 내용은 이 문서를 [참조하세요.](https://aka.ms/OmeEtr)

- 웹에서 Outlook 사용하는 경우 **:** 전자 메일 메시지를 작성하는 경우 OWA에서 **보호를** 클릭합니다. 이렇게 하면 "전달 금지" 권한이 적용됩니다. 권한 **변경을 클릭하고** **암호화를** 클릭하여 메시지만 암호화합니다.

- Outlook 클라이언트를 사용하는 **경우:** Outlook 2013 또는 2016에서 암호화된 메시지를 보내거나 Mac용 Outlook 2016 옵션 사용 권한을 선택하고 필요한 보호 옵션을  >  선택합니다.

- 특정 **받는 사람 또는** 외부 파트너 조직으로 전송되는 모든 전자 메일을 자동으로 암호화하려면 Exchange 관리 센터에서 메일 흐름 전송 규칙을 만들어야 합니다. 자세한 지침은 이 지원 문서 [에서 제공됩니다.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

