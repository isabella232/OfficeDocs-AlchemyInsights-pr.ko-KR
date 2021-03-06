---
title: 조직의 전자 메일 메시지 검색 및 삭제하기
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500967"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>조직의 전자 메일 메시지 검색 및 삭제하기

다음 단계를 따릅니다:

1. 전역 관리자가 아닌 경우 계정을 **eDiscovery 관리자** 역할 그룹 또는 준수 검색 관리 역할에 추가해야 하는 메시지를 **검색합니다.** 메시지를 삭제하려면 조직 관리 역할 그룹  또는 검색 및 제거 관리 역할에 **가입해야 합니다.** 이러한 역할에 대한 사용 권한은 보안 및 준수 & [할당됩니다.](https://protection.office.com)
2. [삭제할 메시지를 찾는](https://docs.microsoft.com/office365/securitycompliance/content-search) 콘텐츠 검색을 생성합니다.
3. [보안 및 준수 센터 PowerShell에 연결](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)합니다. MFA를 사용하는 경우 다음 지침을 참조하세요. 다단계 인증을 & 보안 및 준수 [센터 PowerShell에 연결](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. 메시지 삭제: `New-ComplianceSearchAction` cmdlet을 실행하여 메시지를 삭제합니다. 삭제된 메시지는 사용자의 복구 가능한 항목 폴더로 이동됩니다. 명령의 예는 [3단계: 메시지 삭제를 참조합니다.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
