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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057972"
---
# <a name="create-sharepoint-sites-using-templates"></a>템플릿을 SharePoint 사이트 만들기

최신 통신이나 팀 사이트에서는 사이트를 서식 파일로 저장하는 기능을 지원하지 않습니다. 서식 파일을 사용하는 방법에 대한 자세한 내용은 [SharePoint 사이트를 서식 파일로 저장, 다운로드 및 업로드](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)를 참조하세요.

다음은 Sharepoint Online에서 사이트 또는 목록을 서식 파일로 저장과 관련한 몇 가지 일반적인 문제/해결 방법입니다. 

**사이트/목록 서식 파일 저장 단추를 사용할 수 없는 경우 또는 없는 경우**

관리자는 서식 파일 기능을 사용할 수 있도록 사용자 지정 스크립트를 허용해야 합니다. 자세한 단계, 예제 및 고려 사항은 다음을 참조하세요. 

- [사용자 지정 스크립트 허용 또는 금지](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- 사이트를 서식 파일로 저장 명령이 지원되지 않으며 SharePoint 서버 게시 인프라를 사용하는 사이트에 문제가 발생할 수 있습니다.

**사이트 서식 파일을 만들 수 없는 경우 또는 제대로 작동하지 않습니다.**

템플릿에 기능이 누락될 [](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) 수 있으며 활성화되지 않습니다. 현재 사이트 모음에서 활성화되는 데 해당 기능을 사용할 수 없는 경우, 사이트 서식 파일을 사용하여 사이트를 만들 수 없습니다.

- 목록이나 라이브러리가 [목록 보기 제한 임계값](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)인 5000개 항목을 초과하는지를 확인합니다. 초과하는 경우 사이트 서식 파일을 만들 수 없습니다.

- 사이트에서 너무 많은 리소스를 사용하고 있으므로 사이트 서식 파일이 50MB 제한을 초과합니다.


- 조회 열을 사용하는 목록에서 데이터를 표시하는 데 문제가 있습니다. 자세한 내용은 [서식 파일 생성 목록이 SharePoint Online의 올바른 조회 목록에서 데이터를 표시하지 않음](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)을 참조하세요.

일반적인 문제 및 솔루션에 대한 자세한 내용은 사이트 서식 파일 만들기 [및 사용을 참조하세요.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



