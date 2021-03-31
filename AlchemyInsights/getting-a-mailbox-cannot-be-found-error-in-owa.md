---
title: 126 OWA에서 사서함을 찾을 수 없는 경우
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
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426668"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>웹에서 Outlook에서 사서함을 찾을 수 없는 오류 발생

웹용 Outlook을 사용 중일 때  오류로 사서함을 찾을 수 없는 경우 웹용 Outlook에 연결하는 데 사용한 계정에 Exchange Online 라이선스가 없습니다. 따라서 사서함이 계정과 연결되지 않습니다. 관리자는 다음 단계에 따라 계정에 라이선스를 할당할 수 있습니다.

1. Microsoft [365](https://portal.office.com/adminportal/home#/homepage) 관리 센터를  열고 사용자  섹션에서 활성 사용자로 이동한 다음 오류가 표시하는 사용자를 선택합니다.

2. 열 수 있는 사용자 페이지에서 라이선스  및 앱 섹션으로 이동하여 적절한 위치 값을 선택한 다음 Exchange Online이 포함된 라이선스를 할당합니다(라이선스를 확장하여 세부 정보를 확인).  작업을 마쳤으면 **변경 내용 저장** 을 클릭합니다.

경우에 따라 라이선스가 사용자 계정에 이미 할당된 경우 라이선스를 제거하고 다시 할당하면 문제를 해결하고 시스템에 올바르게 프로비전하는 데 도움이 됩니다. 

- M365 Exchange Online 및 기타(있는 경우) 구독이 현재 있으며 최근에 만료되지 않은지 확인할 수 있습니다.

구독이 만료되지 않고 유효한 라이선스가 사용자 계정에 할당된 경우 라이선스가 프로비전되는 데 최대 24시간이 걸릴 수 있으므로 문제가 해결될 때까지 기다려야 할 수 있습니다. 자세한 내용은 라이선스 할당 및 [관리를 참조하세요.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)