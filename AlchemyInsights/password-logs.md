---
title: 암호 로그
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ab2899cc96fb76705665eff4a535de5ada5bc4dd733723349a6fb649adfb034b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960949"
---
# <a name="password-logs"></a>암호 로그

**암호 재설정 감사 로그에 액세스하는 데 문제가 있습니다.**

암호 재설정 감사 로그 액세스와 관련한 문제를 해결하려면 다음 단계를 수행하세요.

감사 로그를 볼 권한이 있는지 확인합니다. 

다음 역할에 한해 권한이 있습니다.
 - 전역 관리자
 - 보안 관리자
 - 보안 읽기 권한자

**처음 배포한 때로부터 모든 암호 재설정 감사 이벤트를 보려는 경우**

최근 30일에 해당하는 보고서에 최대 120,000개의 암호 재설정/등록 이벤트가 저장됩니다. 이 최대 한도는 CSV를 다운로드할 때 UI에 적용됩니다. PowerShell을 통해 1백만 개 이벤트가 제공됩니다.
자세한 내용은 다음 링크를 참조하세요.

- [Azure AD 보고서 및 이벤트 API의 셀프 서비스 암호 재설정 이벤트](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [PowerShell을 사용하여 빠르게 암호 재설정 등록 이벤트를 다운로드하는 방법](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**암호 재설정 보고 기능에 대한 자세한 정보를 알고 싶은 경우**

Microsoft Azure portal의 **사용자 및 그룹** 에서 Azure AD 암호 재설정 감사 로그를 사용하여 암호를 등록하거나 재설정하는 사람을 확인합니다.
자세한 내용은 다음 링크를 참조하세요.

- [암호 재설정 보고서 개요](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Azure Portal에서 암호 재설정 보고서를 보는 방법](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Azure AD 보고서 및 이벤트 API의 셀프 서비스 암호 재설정 이벤트](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [PowerShell을 사용하여 빠르게 암호 재설정 등록 이벤트를 다운로드하는 방법](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


