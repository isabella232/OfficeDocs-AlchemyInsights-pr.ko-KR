---
title: 클래식 SharePoint 감사 로그 보고서
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509606"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint 및 OneDrive 감사 로그

## <a name="sharepoint-classic-audit-logs"></a>SharePoint 클래식 감사 로그

SPO 레거시 감사가 UAL (통합 감사 로그)로 마이그레이션 되었습니다. 이제 모든 SPO 레거시 감사 보고서가 UAL를 통해 켜 지 며 레거시 감사 신호가 UAL로 마이그레이션 되었습니다.

주요 변경 사항:

* 자르기는 기능으로 사용할 수 없습니다.
* 감사할 특정 이벤트 선택이 가능 하지 않습니다. 기본적으로 사용할 수 있는 감사 이벤트의 전체 목록을 보려면 [이 문서](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) 를 참조 하십시오.
* **사용자 지정 된 보고서** 에서 **위치** 옵션을 사용할 수 없습니다.
* **문서 열기 또는 다운로드** 옵션은 사용할 수 없습니다.

[사이트 모음에 대 한 감사 설정 구성](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint 및 OneDrive 최신 통합 감사 로그 (규정 준수)

* [통합 감사 로깅 설정/해제](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

SharePoint 또는 OneDrive 내에 추가 구성은 필요 하지 않습니다.

감사 로깅 검색을 사용 하 여 파일 (s), 폴더, 사용자의 사용 권한 작업을 확인 합니다.

* [파일 및 페이지 활동](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [폴더 활동](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [공유 및 액세스 요청 활동](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [동기화 활동](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [사이트 관리 활동](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

이러한 이벤트를 검색 하는 방법에 대 한 자세한 내용은 [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)을 참조 하십시오.
