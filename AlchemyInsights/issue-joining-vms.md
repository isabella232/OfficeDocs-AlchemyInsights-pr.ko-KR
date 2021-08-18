---
title: VM 조인 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: d89fb92ce1775e5a77808a1893a315419b4d54706dc737327c51f7c4c4e488e2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088078"
---
# <a name="issue-joining-vms"></a>VM 조인 문제

VM을 조인하는 동안 발생하는 문제를 해결하려면 다음 단계를 수행하세요.

1. **SAMAccountName** 형식 대신 **UPN** 형식(예: 'joeuser@contoso.com')을 사용하여 로그인합니다.
2. *시작 가이드* 에 설명된 단계에 따라 암호 동기화를 사용 가능으로 설정했는지 확인합니다.
3. 영향을 받는 사용자 계정이 Azure AD 테넌트의 외부 계정이 아닌지 확인하세요. Azure AD Domain Services에는 이러한 사용자 계정에 대한 자격 증명이 없기 때문에 외부 사용자가 관리 도메인에 로그인할 수 없습니다.
4. 영향을 받는 사용자 계정이 클라우드 전용 사용자 계정인 경우 Azure AD Domain Services를 사용하도록 설정한 후 사용자가 암호를 변경했는지 확인하십시오. 이 단계에서는 Azure AD Domain Services를 생성하는 데 필요한 자격 증명 해시를 생성합니다.
5. 영향을 받는 사용자 계정이 온-프레미스 디렉토리에서 동기화되는 경우 Azure AD Connect의 권장 릴리스가 전체 동기화를 수행하도록 구성되었는지 확인합니다.
6. 4단계를 확인한 후에도 문제가 지속되면 동기화 시스템에서 다음 명령을 실행합니다.
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.