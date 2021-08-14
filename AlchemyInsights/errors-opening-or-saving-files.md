---
title: 파일 열기 또는 저장 오류
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000583"
- "2685"
ms.openlocfilehash: 13a75338e3784d3df2ec93e8096380f85494317b7161040c7ad60ad830f9211d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978095"
---
# <a name="resolve-errors-opening-or-saving-word-files"></a>Word 파일 열기 또는 저장 오류 해결

Word 문서를 열거나 저장하는 데 문제가 있는 경우 다음을 시도합니다.

- [업데이트 Office 설치합니다.](https://support.office.com/article/2ab296f3-7f03-43a2-8e50-46de917611c5) 최신 업데이트 목록은 Office [업데이트 를 참조하세요.](https://docs.microsoft.com/officeupdates/office-updates-msi)
- [Word에서 손상된 문서 문제를 해결합니다.](https://docs.microsoft.com/office/troubleshoot/word/damaged-documents-in-word)
- [응용 Office 복구합니다.](https://support.office.com/Article/Repair-an-Office-application-7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)
- 문서에 변경 내용이 포함된 경우 문제를 해결하기 위해 과도한 변경 내용이나 설명이 있는 경우 [Word의](https://docs.microsoft.com/office/troubleshoot/word/word-stops-responding) 제안이 느려지거나 응답하지 않습니다.

다음 중 하나와 같은 오류가 발생하면 레지스트리 정책 설정에 의해 파일이 Office 오류 메시지의 [제안을 사용합니다.](https://docs.microsoft.com/office/troubleshoot/settings/file-blocked-in-office)

- 레지스트리 정책 설정에 의해 차단된 파일 형식을 열려고 합니다.
- 보안 센터의 파일 설정에 의해 차단된 파일 형식 **\<File Type\>** 을 열려고 합니다.
- 이전 버전의 Microsoft Office에서 만든 파일을 열려고 합니다. 레지스트리 정책 설정에 따라 이 버전에서는 이 파일 형식을 열 수 없습니다.
- 레지스트리 정책 설정에 의해 차단된 파일을 저장하려고 합니다.
- 보안 센터의 파일 차단 설정에 의해 차단된 파일 형식을 저장하려고 합니다.

SharePoint 또는 OneDrive 문서 라이브러리에서 Office 파일을 여는 데 문제가 있는 경우 다음을 시도해 보세요.

- 파일이 지원되는지 확인하기 위해 [OneDrive, 비즈니스용 OneDrive 및 SharePoint의 잘못된 파일 이름 및 파일 형식](https://support.office.com/article/64883a5d-228e-48f5-b3d2-eb39e07630fa)을 확인하세요. 
- [Office 문서 캐시를 삭제하세요](https://support.office.com/article/b1d3765e-d71b-4bb8-99ca-acd22c42995d
). 

자세한 내용은 [SharePoint 라이브러리에서 문서를 열 때 발생하는 문제 해결하기](https://support.office.com/article/31329fa1-4ad0-47fc-95d8-bb0c5b12a536)를 참조하세요.