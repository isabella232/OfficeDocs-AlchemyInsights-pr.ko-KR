---
title: 외부 자동 전자 메일 전달 차단 또는 차단 해제
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
ms.openlocfilehash: 6c4ddd53ab794ffad3179dd86a8f81785567cfe34240dff2aa0a1df11094883d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897474"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>자동 전자 메일 전달 차단 또는 차단 해제

특정 사서함에 대해 전자 메일 전달을 사용하도록 설정하거나 사용하지 않도록 설정하려면 전자 메일 전달 [구성을 참조하세요.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

관리자는 아웃바운드 스팸 정책을 사용하여 조직의 외부 [전달을 제어할 수 있습니다.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) <https://security.microsoft.com/antispam>PowerShell에서 [get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) cmdlet을 사용하여 Microsoft 365 Defender 포털에서 아웃바운드 스팸 정책을 Exchange Online 있습니다.

**"550 5.7.520 액세스가** 거부되어 조직에서 외부 전달을 허용하지 않습니다."라는 오류가 표시되면 정책이 외부 자동 전달 메시지를 사용하도록 구성되어 있는지 확인 합니다.

**참고:** 기본 아웃바운드 스팸 필터  정책(자동 외부 전달이 차단되어 내부 자동 전달이 계속 작동)에서 자동 전달 규칙 설정에 대해 시스템 제어 기본값을 권장했습니다.  사용자 지정 아웃바운드 스팸 필터 정책을 만들고 **On - Forwarding은** 외부 자동 전자 메일 전달이 필요한 사용자에 한해 사용하도록 설정됩니다. 자세한 내용은 에서 외부 전자 메일 전달 [구성을 Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)
