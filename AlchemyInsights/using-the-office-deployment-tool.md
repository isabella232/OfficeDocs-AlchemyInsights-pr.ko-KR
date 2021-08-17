---
title: Office 배포 도구 사용
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083776"
---
# <a name="using-the-office-deployment-tool-odt"></a>ODT(Office 배포 도구) 사용

ODT(Office 배포 도구)를 사용하여 OFFICE 365 버전을 배포할 Office. Office 배포 도구(setup.exe)는 명령줄에서 실행되어 구성 XML 파일을 사용하여 배포할 때 적용할 설정을 Office.
  
1. Microsoft 다운로드 센터에서 Office 배포 도구의 최신 버전을 [다운로드합니다.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. [OCT(Office 사용자](https://config.office.com) 지정 도구)를 사용하여 배포 기본 설정을 선택하고 구성 XML 파일을 만들 수 있습니다. 구성 파일을 내보내고 구성 파일이 있는 동일한 폴더에 setup.exe 배치합니다.

    **참고:** Office 구성 파일이 잘못 구성되어 설치 문제가 자주 발생합니다. 이러한 문제를 방지하려면 Office 사용자 지정 도구를 사용하여 구성 파일을 만드는 것이 좋습니다. 기존 구성 파일을 사용자 지정 도구의 Office 있습니다.

3. 상승된 명령 프롬프트에서 setup.exe 위치로 전환하고 다운로드 모드에서 Office 배포 도구를 실행하고 방금 저장한 구성 파일을 지정합니다. 이 예제에서는 구성 파일의 이름이 다음과 Configuration.xml.

```setup.exe /download Configuration.xml```

4.Office 배포 도구를 구성 모드에서 실행하고 구성 파일을 지정합니다.

```setup.exe /configure Configuration.xml```

**참고:** 설치하려는 클라이언트 컴퓨터에서 이 단계를 실행해야 Office 해당 컴퓨터에 대한 로컬 관리자 권한이 있어야 합니다.

Office 배포 시나리오에 엔터프라이즈용 Microsoft 365 앱 배포 도구 사용에 대한 자세한 내용은 [Overview of the Office Deployment Tool를 참조하십시오.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Office 사용자 지정 도구를 사용하는 방법에 대한 자세한 내용은 Office 사용자 지정 도구 [개요를 참조하십시오.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
