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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478322"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>전자 메일 전달 차단 또는 차단 해제

특정 사서함에 대해 전자 메일 전달을 사용 하거나 사용 하지 않도록 설정 하려면 [전자 메일 전달 구성을](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)참조 하십시오.

테 넌 트 수준에서 외부 전달을 제어 하는 작업은 아웃 바운드 스팸 정책을 사용 하 여 수행 됩니다. [여기](https://protection.office.com/antispam) 에서 또는 [Get-get-hostedoutboundspamfilterpolicy 명령을](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)사용 하 여 보안 및 준수 센터에서 아웃 바운드 스팸 필터 정책을 확인할 수 있습니다.

**"550 5.7.520 액세스 거부, 조직에서 외부 전달을 허용 하지 않습니다." 라는**오류가 나타나면 정책이 외부 자동 전달을 사용 하도록 구성 되어 있는지 확인 하십시오.

**참고:** 기본 아웃 바운드 스팸 필터 정책에서 외부 Autoforward을 사용 하지 않도록 설정 하 고 해당 사용자에 대 한 사용자 지정 정책을 만들어 외부 전달을 필요로 하는 사용자에 대해서만 사용 하도록 설정 하는 것이 좋습니다. [Office 365에서 외부 전자 메일 전달 구성](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)에 대 한 자세한 내용을 확인할 수 있습니다.