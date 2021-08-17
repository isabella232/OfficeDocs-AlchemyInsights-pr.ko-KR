---
title: 암호 정책
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040836"
---
# <a name="password-policies"></a>암호 정책

**사용자의 암호 정책에 문제가 있습니다.**

- 사용자의 암호 정책은 사용자가 클라우드 전용인지 아니면 사내에 있는지에 따라 결정됩니다.
- 클라우드 전용 사용자는 이 문서의 요구 사항을 충족하는 암호를 [선택해야](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts) 합니다. 클라우드 사용자 계정에만 적용되는 암호 정책
- On-premises users must choose a password that meet the on-premises requirements. 프레미스 사용자가 암호를 설정할 수 없는 경우, On-premises requirements을 확인합니다.

**암호 만료 정책을 설정하거나 검사하는 방법을 모르는 경우**

- PowerShell을 사용하여 테넌트의 클라우드 사용자에 대한 만료 정책을 설정하고 확인할 수 있습니다. 이 문서의 지침에 따라 [PowerShell을](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell) 사용하여 암호 정책 설정 또는 확인
- On-premises 사용자에 대한 암호 만료 정책은 프레미스 AD에서 설정됩니다.

**기타 유용한 링크:**
- [암호 재설정 시작](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [관리자가 시작한 암호 재설정 문제 해결](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
