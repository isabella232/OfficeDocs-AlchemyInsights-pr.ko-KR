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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219861"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>전자 메일 전달 차단 또는 차단 해제

특정 사서함에 대해 전자 메일 전달을 사용 하거나 사용 하지 않도록 설정 하려면 [전자 메일 전달 구성을](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)참조 하십시오.

테 넌 트 수준에서는 아웃 바운드 스팸 방지 정책을 사용 하 여 외부 전달 제어를 수행 합니다. 이 설정이 해제 또는 자동으로 설정 된 경우에는 "550 5.7.520 액세스 거부, 조직에서 외부 전달을 허용 하지 않습니다." 라는 오류가 발생 하 여 전자 메일 전달이 차단 될 수 있습니다. 나중에 전달이 차단 되도록 설정 된 경우 사용자에 게 표시 되는 오류입니다.

전달이 차단 되는 경우에는 정책이 외부 Autoforward을 사용 하도록 구성 되어 있는지 확인 하세요. 아웃 바운드 스팸 필터 정책을 보안 및 준수 센터에서 확인 하거나 command Get-Get-hostedoutboundspamfilterpolicy |를 실행 하 여 확인할 수 있습니다. fl name, AutoForwardingMode Autoforward 차단을 설정 하려는 경우 동일한 명령을 실행 하면 이제 정책의 상태를 확인할 수 있습니다.

참고: 외부 Autoforward를 기본 아웃 바운드 스팸 필터 정책에서 사용 하지 않도록 설정 하 고 해당 사용자에 대 한 사용자 지정 정책을 만들어 외부 전달을 필요로 하는 사용자에 대해서만 사용 하도록 설정 하는 것이 좋습니다. [Office 365에서 외부 전자 메일 전달 구성](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)에 대 한 자세한 내용을 확인할 수 있습니다.