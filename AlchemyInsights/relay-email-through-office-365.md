---
title: Microsoft 365를 통해 전자 메일 릴레이
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117989"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>전자 메일을 보내도록 다기능 장치 또는 애플리케이션 설정

옵션 및 단계에 대한 자세한 내용은 [Microsoft 365를 사용하여 전자 메일을 보내도록 다기능 장치 또는 애플리케이션을 설정하는 방법](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)을 참조하세요.
  
최근에 작동이 중지된 디바이스 또는 애플리케이션이 있는 경우 가장 일반적인 문제는 다음과 같습니다.

- **SMTP 인증 클라이언트 제출을 사용하는 동안 발생하는 인증 관련 오류** 최근에 SMTP 인증 작동 방식과 관련된 몇 가지 사항이 변경되었습니다. 문제를 해결하는 방법에 대한 자세한 내용은 [Microsoft 365 또는 Office 365를 사용하여 전자 메일을 보내는 프린터, 스캐너 및 LOB 응용 프로그램의 문제 해결](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)의 인증 실패 섹션을 참조하세요.
- **Microsoft는 Office 365에 안전하게 연결하는 동안 TLS 1.2 버전만 허용합니다** TLS(보안 연결)를 사용하는 경우 애플리케이션 장치가 TLS 1.2를 지원하는지 확인합니다. 자세한 내용은 [Office 365 및 Office 365 GCC에서 TLS 1.2 준비](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)를 참조하세요.
 
기타 문제 및 해결 방법은 [Microsoft 365 또는 Office 365를 사용하여 전자 메일을 보내는 프린터, 스캐너 및 LOB 애플리케이션의 문제 해결](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)을 참조하세요.

영향을 받는 장치를 보려면 [SMTP 인증 클라이언트 보고서](https://protection.office.com/mailflow/dashboard)로 이동합니다.

**참고**: Exchange Online은 대량 메일 시나리오를 수용하지 않습니다. 대량 상업용 이메일(예: 고객 뉴스레터)을 보내려면 이러한 서비스를 전문으로 하는 타사 제공자를 사용해야 합니다.
