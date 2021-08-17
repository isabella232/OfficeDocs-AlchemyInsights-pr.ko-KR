---
title: 726 전자 메일 전달 차단
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059638"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>전자 메일 전달 차단 또는 차단 해제

특정 사서함에 대해 전자 메일 전달을 사용하도록 설정하거나 사용하지 않도록 설정하려면 전자 메일 전달 [구성을 참조하세요.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

테넌트 수준에서 외부 전달 제어는 아웃바운드 스팸 정책을 사용하여 수행됩니다. 여기에서 또는 [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)명령을 사용하여 보안 및 준수 센터에서 아웃바운드 스팸 필터 정책을 확인할 수 있습니다. [](https://protection.office.com/antispam)

**"550 5.7.520 액세스가** 거부되어 조직에서 외부 전달을 허용하지 않습니다."라는 오류가 발생하는 경우, 외부 자동 전달을 사용하도록 정책이 구성되어 있는지 확인하시기 바랍니다.

**참고:** 기본 아웃바운드 스팸 필터 정책에서 외부 자동 적용을 사용하지 않도록 설정하고 해당 사용자에 대한 사용자 지정 정책을 만들어 외부 전달이 필요한 사용자에 한해 외부 자동 전달을 사용하도록 설정하는 것이 좋습니다. 자세한 내용은 에서 [Configuring external email forwarding in Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)