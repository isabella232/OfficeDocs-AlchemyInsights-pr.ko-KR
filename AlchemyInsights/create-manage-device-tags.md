---
title: 디바이스 태그 또는 그룹 만들기 및 관리
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: c06fbd377159e55cf34c79ef0aa1e34f0412a908e8d4e3dec5ad088c9b8b818a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898206"
---
# <a name="create-and-manage-device-tags-or-groups"></a>디바이스 태그 또는 그룹 만들기 및 관리

디바이스에 태그를 추가하여 논리적 그룹 소속을 만듭니다. 디바이스 태그는 네트워크의 적절한 매핑을 지원하므로 다양한 태그를 연결하여 컨텍스트를 캡처하고 인시던트 일부로 동적 목록 만들기를 사용하도록 설정할 수 있습니다. 태그는 디바이스 목록 보기에서 필터로 사용하거나 디바이스를 그룹화하는 데 사용할 수 있습니다. 디바이스 그룹화에 대한 자세한 내용은 [디바이스 태그 만들기 및 관리를](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/machine-tags) 참조하세요.

다음을 수행하여 디바이스에 태그를 추가할 수 있습니다.

- 포털 사용

- 레지스트리 키 값 설정
 
**참고:** 태그가 디바이스에 추가되는 시간과 디바이스 목록 및 디바이스 페이지의 가용성 사이에 대기 시간이 있을 수 있습니다.

API를 사용하여 디바이스 태그를 추가하려면 [디바이스 태그 API 추가 또는 제거](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)를 참조하세요.

## <a name="add-and-manage-device-tags-using-the-portal"></a>포털을 사용하여 디바이스 태그 추가 및 관리

1. 태그를 관리할 디바이스를 선택합니다. 다음 보기 중 하나에서 디바이스를 선택하거나 검색할 수 있습니다.

    - **보안 작업 대시보드** 활성 경고가 있는 상위 디바이스에서 디바이스 이름을 선택하세요.
    - **경고 큐** - 경고 큐에서 디바이스 아이콘 옆에 있는 디바이스 이름을 선택하세요.
    - **디바이스 목록** - 디바이스 목록에서 디바이스 이름을 선택하세요.
    - **검색 상자** - 드롭다운 메뉴에서 디바이스를 선택하고 디바이스 이름을 입력하세요.

    파일 및 IP 보기를 통해 경고 페이지로 이동할 수도 있습니다.

1. 응답 작업 행에서 **태그 관리** 를 선택하세요.

1. 찾거나 만드려는 태그 입력

태그는 디바이스 보기에 추가되고 디바이스 목록 보기에 반영됩니다. 그런 다음에는 태그 필터를 사용하여 관련 디바이스 목록을 볼 수 있습니다.

자세한 내용은 [디바이스 태그 만들기 및 관리](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/machine-tags)을 참조하세요.