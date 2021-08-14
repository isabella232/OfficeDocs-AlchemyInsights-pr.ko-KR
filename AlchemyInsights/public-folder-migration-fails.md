---
title: 95%에서 공용 폴더 마이그레이션이 실패함
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: e92a983a74ac0b97a613723dacb356ebff68f6cdba2d78ca63085a818d12e739
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923317"
---
# <a name="public-folder-migration-fails-at-95"></a>95%에서 공용 폴더 마이그레이션이 실패함

마이그레이션 일괄 완료를 시작했을 수 있으며 마이그레이션 일괄 상태가 매우 오랫동안 **동기화됨** 으로 계속 표시됩니다. 이는 예상된 동작입니다.

일반적으로 마이그레이션 일괄 처리의 상태가 **완료** 로 전환되기 전에 몇 시간 동안 **동기화** 상태로 남아있습니다. 다수의 대상 사서함이 포함된 마이그레이션의 경우 기본 공용 폴더 마이그레이션 요청이 실패하거나 격리되지 않은 경우 마이그레이션 일괄 처리의 상태는 일반적으로 24시간 이상 동기화 상태로 남아있습니다. 마이그레이션 일괄 처리가 완료될 때까지 24~48시간 기다리세요.

FailedToMailEnablePublicFoldersException 오류에 의해 95%에서 실패하는 공용 폴더 마이그레이션:

1. Exchange 온-프레미스 서버에서 [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) 스크립트를 다운로드하고 실행합니다.

2. 스크립트가 제안한 수정 조치를 수행합니다.

3. Sync-MailPublicFolders(Exchange 2010의 경우) 또는 Sync-ModernMailPublicFolders(Exchange 2013 이상)를 실행합니다.

4. 공용 폴더 마이그레이션을 다시 시작합니다.
