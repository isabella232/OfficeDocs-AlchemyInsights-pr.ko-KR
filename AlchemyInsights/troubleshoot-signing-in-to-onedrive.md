---
title: OneDrive로의 로그인 문제 해결
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8283"
- "9004614"
ms.openlocfilehash: 2c9a390f38ecbba94698a352348e2e533a50ee17
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52626119"
---
# <a name="troubleshoot-signing-in-to-onedrive"></a>OneDrive로의 로그인 문제 해결

이 문서에서는 다음과 같은 시나리오에 대해 설명합니다.

- OneDrive 동기화 클라이언트에 로그인하는 문제 해결
- 비즈니스용 OneDrive 사이트에 로그인하는 문제 해결

**OneDrive 동기화 클라이언트에 로그인하는 문제 해결**

- 오류 코드 0x004de40을 해결하는 단계는 [OneDrive에 로그인할 때 발생하는 오류 코드 0x8004de40](/sharepoint/troubleshoot/administration/error-0x8004de40-in-onedrive)을 참조하세요.
- 사이트를 방문하여 OneDrive 또는 SharePoint 사이트에 로그인하고 사이트의 메뉴 막대 맨 위에 있는 **동기화** 단추를 클릭합니다.
- OneDrive.com이 아니라 비즈니스용 OneDrive에 로그인하고 있는지 확인합니다. 방문하는 URL이 onedrive.live.com으로 시작한다면 해당 사이트는 비즈니스용 OneDrive를 위한 위치가 아닙니다. 비즈니스용 OneDrive에 로그인하는 간단한 방법은 이 링크https://portal.office.com/onedrive를 사용한 다음, 회사 또는 학교 계정을 사용하여 로그인하는 것입니다.
- 계속 문제가 있는 경우 [OneDrive를 다시 설정](https://support.microsoft.com/office/reset-onedrive-34701e00-bf7b-42db-b960-84905399050c)해 보세요.
- [OneDrive에서 계정 연결을 해제](https://support.microsoft.com/office/how-to-remove-an-account-in-onedrive-72699268-9e64-45bd-b723-9a19f4512fd1)하고 OneDrive 또는 SharePoint 사이트에 로그인한 다음 사이트의 메뉴 모음 상단에 있는 **동기화** 버튼을 클릭합니다.

**비즈니스용 OneDrive 사이트에 로그인하는 문제 해결**

- OneDrive.com이 아니라 비즈니스용 OneDrive에 로그인하고 있는지 확인합니다. 방문하는 URL이 onedrive.live.com으로 시작한다면 해당 사이트는 비즈니스용 OneDrive를 위한 위치가 아닙니다. 비즈니스용 OneDrive에 로그인하는 간단한 방법은 이 링크https://portal.office.com/onedrive를 사용한 다음, 회사 또는 학교 계정을 사용하여 로그인하는 것입니다.
- Delve 프로필 페이지로 리디렉션되는 경우 Microsoft 365 관리자는 [사용자에게 비즈니스용 OneDrive 사이트를 생성할 수 있는 권한을 부여](https://support.microsoft.com/office/you-re-redirected-to-your-delve-profile-page-after-you-click-onedrive-on-the-microsoft-365-app-launcher-2af26640-9ddf-46c3-8912-6af30efcc7b0)해야 합니다.
- [Microsoft Edge에서 InPrivate 브라우징](https://support.microsoft.com/microsoft-edge/browse-inprivate-in-microsoft-edge-e6f47704-340c-7d4f-b00d-d0cf35aa1fcc)(또는 다른 브라우저의 유사한 기능)을 사용하여 OneDrive 사이트를 방문할 수 있는지 테스트합니다.
    - InPrivate 브라우징이 작동하는 경우 [Microsoft Edge(또는 다른 브라우저의 유사한 기능)에서 검색 데이터를 지워야](https://support.microsoft.com/microsoft-edge/view-and-delete-browser-history-in-microsoft-edge-00cf7943-a9e1-975a-a33d-ac10ce454ca4)할 수 있습니다.

**OneDrive와 동기화하기 위한 Office로의 로그인 문제 해결**

**업로드 차단됨**, **이 파일을 저장하도록 로그인** 또는 **복사본 저장** 오류 메시지가 표시되는 경우, [Office에 연결된 서비스에서 OneDrive를 제거하고 다시 연결](https://support.microsoft.com/office/how-to-resolve-upload-blocked-sign-into-save-this-file-or-save-a-copy-error-messages-32c7340c-f5fb-4ca0-a829-65d8120f81f8)해야 할 수 있습니다.

**기타 문제 해결 팁**

전역, 라이선스 또는 사용자 관리자일 경우 영향을 받는 사용자에게 [올바른 라이선스를 할당](/microsoft-365/admin/manage/assign-licenses-to-users)합니다.

