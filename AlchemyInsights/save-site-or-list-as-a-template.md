---
title: 사이트 또는 목록을 서식 파일로 저장
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109210"
---
# <a name="save-site-or-list-as-a-template"></a>사이트 또는 목록을 서식 파일로 저장

SharePoint 사이트 서식 파일은 특정 비즈니스 필요성을 중심으로 설계된 미리 작성된 정의입니다. 자세한 내용은 서식 파일을 사용하여 다양한 종류의 사이트 [만들기를 SharePoint 참조하세요.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

다음은 사이트 또는 목록을 온라인에서 서식 파일로 저장하는 방법에 대한 몇 가지 일반적인 문제/SharePoint 있습니다.

**사이트/목록 서식 파일 저장 단추를 사용할 수 없습니다.** 

- 관리자는 서식 파일 기능을 사용할 수 있도록 사용자 지정 스크립트를 허용해야 합니다. 자세한 단계, 예제 및 고려 사항은 사용자 지정 스크립트 [허용 또는 금지를 참조하세요.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- 사이트를 서식 파일로 저장 명령이 지원되지 않으며 SharePoint 서버 게시 인프라를 사용하는 사이트에 문제가 발생할 수 있습니다.


**사이트 서식 파일을 만들 수 없는 경우 또는 제대로 작동하지 않습니다.**

- 템플릿에 기능이 누락될 [](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) 수 있으며 활성화되지 않습니다. 현재 사이트 모음에서 활성화되는 데 해당 기능을 사용할 수 없는 경우, 사이트 서식 파일을 사용하여 사이트를 만들 수 없습니다.


- 목록이나 라이브러리가 [목록 보기 제한 임계값](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)인 5000개 항목을 초과하는지를 확인합니다. 초과하는 경우 사이트 서식 파일을 만들 수 없습니다.


- 사이트가 너무 많은 리소스를 사용하고 있을 수 있으므로 사이트 서식 파일은 50MB 제한을 초과합니다.


- 조회 열을 사용하는 목록에서 데이터를 표시하는 데 문제가 있습니다. 자세한 내용은 [Template-generated list doesn't display data from the correct lookup list in SharePoint.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)


일반적인 문제 및 솔루션에 대한 자세한 내용은 사이트 서식 파일 만들기 및 사용을 [참조하세요.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

