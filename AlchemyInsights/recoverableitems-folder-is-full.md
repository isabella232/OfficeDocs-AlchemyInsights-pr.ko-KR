---
title: 1336 RecoverableItems 폴더가 가득 습니다.
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061762"
---
# <a name="the-recoverable-items-folder-is-full"></a>복구할 수 있는 항목 폴더가 가득 습니다.

Exchange Online 사서함의 경우 복구 가능한 항목 폴더의 기본 저장소 제한은 30GB입니다. 사서함에 소송 보존, eDiscovery 보류가 적용되거나 보존 정책에 할당된 경우 복구 가능한 항목 폴더의 저장소 제한이 자동으로 100GB로 증가합니다.

복구 가능한 항목 폴더가 저장소 제한에 도달하면 사서함 기능이 다음과 같은 방식으로 영향을 받는 것입니다.

- 사용자는 사서함에서 항목을 삭제할 수 없습니다.

- 관리되는 폴더 도우미는 보존 태그 또는 관리되는 폴더 설정에 따라 항목을 삭제할 수 없습니다.

- 단일 항목 복구를 사용하도록 설정하거나 보류된 사서함의 경우 기록 중 복사 페이지 보호 프로세스는 사용자가 편집한 항목 버전을 유지 관리하지 못합니다.

- 사서함 감사 로깅을 사용하도록 설정한 사서함의 경우 복구 가능한 항목 폴더의 감사 하위 폴더에 사서함 감사 로그 항목을 저장할 수 없습니다.

보류되지 않은 사서함의 경우 관리자는 PowerShell에서 Exchange Online 명령을 사용하여 복구 가능한 항목 폴더의 항목을 `Search-Mailbox -SearchDumpsterOnly -DeleteContent` 삭제할 수 있습니다. 자세한 내용은 아래 항목을 참조하세요.

- [메시지 검색 및 삭제](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

보류된 사서함의 경우 관리자가 복구 가능한 항목 폴더에서 항목을 삭제하려면 먼저 보류를 제거해야 합니다. 자세한 내용은 클라우드 기반 사서함의 복구 가능한 항목 폴더에서 항목 삭제 보류를 [참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

복구 가능한 항목 폴더가 가득 차지 않도록 관리자는 보류된 사서함에 대한 복구 가능한 항목 폴더의 저장소 제한을 늘리고 복구 가능한 항목 폴더에서 사용자의 보관 사서함으로 항목을 이동하는 사서함 보존 정책을 설정할 수 있습니다. 보류된 사서함에 대한 복구 가능한 항목 할당량 [늘리기 를 참조합니다.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
