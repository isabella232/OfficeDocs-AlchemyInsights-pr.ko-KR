---
title: Microsoft 365 관리 센터의 보고서에 읽을 수 있는 사용자 이름이 표시되지 않음
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/04/2021
ms.locfileid: "58896349"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Microsoft 365 관리 센터의 보고서에 읽을 수 있는 사용자 이름이 표시되지 않음

Microsoft 365 관리 센터의 보고서에 사용자 이름이 표시되지 않지만 대신 B2BC6C15BB9FCDEA71E5CD302D228CC8과 같은 영숫자 값이 표시됩니다.

이는 예상된 동작이며 메시지 센터(MC275344, 2021년 8월 3일 게시)에 전달되었습니다. 

전역 관리자는 조직 개인 정보 보호 관행이 허용하는 경우 테넌트에 대해 이 변경 사항을 되돌리고 식별 가능한 사용자 정보를 표시할 수 있습니다. 테넌트의 변경 내용을 되돌리려면 다음을 수행합니다.

1. 관리 센터에서 **설정** > **조직 설정** > [**서비스**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services)로 이동하고 **보고서** 를 선택합니다. 
1. **사용자 정보 표시 방법 선택** 에서 **보고서에 식별 가능한 사용자 정보 표시** 를 선택한 다음 보고서를 다시 실행합니다.