---
title: SharePoint Online에서 사이트 만들기
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732236"
---
# <a name="create-sharepoint-sites-using-templates"></a>템플릿을 사용 하 여 SharePoint 사이트 만들기

사이트를 서식 파일로 저장 하는 기능은 최신 통신 또는 팀 사이트에서는 지원 되지 않습니다. 서식 파일을 사용 하는 방법에 대 한 자세한 내용은 [저장 및 다운로드 하 여 SharePoint 사이트를 서식 파일로 업로드를](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)참조 하세요.

다음은 Sharepoint Online에서 사이트 또는 목록을 서식 파일로 저장 하는 방법에 대 한 몇 가지 일반적인 문제/해결 방법입니다. 

**사이트 저장/목록 서식 파일 단추를 사용할 수 없거나 누락 되었습니다.**

관리자는 서식 파일 기능을 사용 하도록 설정 하기 위해 사용자 지정 스크립트를 허용 해야 합니다. 자세한 단계는 예 및 고려 사항 참조 

- [사용자 지정 스크립트 허용 또는 금지](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- 사이트를 서식 파일로 저장 명령은 지원 되지 않으며 SharePoint Server 게시 인프라를 사용 하는 사이트에서 문제를 발생 시킬 수 있습니다.

**사이트 서식 파일을 만들 수 없거나 제대로 작동 하지 않음**

서식 파일에 [기능이](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) 누락 되었거나 활성화 되지 않을 수 있습니다. 현재 사이트 모음에서 정품 인증 기능을 사용할 수 없는 경우에는 사이트 서식 파일을 사용 하 여 사이트를 만들 수 없습니다.

- 목록 또는 라이브러리가 사이트 서식 파일의 생성을 차단할 수 있는 것으로 표시 되는 것으로 5000 항목의 [목록이](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 나 라이브러리를 초과 하는지 확인 합니다.

- 사이트에서 너무 많은 리소스를 사용 하 고 있기 때문에 사이트 서식 파일이 50 MB 제한을 초과 합니다.


- 조회 열을 사용 하는 목록의 데이터를 표시 하는 데 문제가 있습니다. 자세한 내용은 [Template 생성 목록에서 SharePoint Online의 올바른 조회 목록의 데이터를 표시 하지 않습니다](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).를 참조 하세요.

일반적인 문제와 솔루션에 대 한 자세한 내용은 [사이트 서식 파일 만들기 및 사용](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)을 확인 하세요.



