---
title: ODT(Office 배포 도구) 사용 방법에 대한 질문
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959689"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>ODT(Office 배포 도구) 사용 방법에 대한 질문

Office 배포 도구를 [Microsoft 다운로드 센터](https://go.microsoft.com/fwlink/p/?LinkID=626065)에서 다운로드합니다.
  
파일을 다운로드한 후에 Office 배포 도구 실행 파일(setup.exe) 및 샘플 구성 파일(configuration.xml)이 포함된 자동 압축 풀기 실행 파일을 실행합니다.
  
 **클라이언트 컴퓨터에서 엔터프라이즈용 Microsoft 365 앱 제품을 제외하거나 제거하려면**
  
설치 시 엔터프라이즈용 Microsoft 365 앱 제품을 제외할 수 있습니다. 이렇게 하려면 ODT를 사용하여 Office를 설치하기 위한 단계를 수행하되 구성 파일에 ExcludeApp 요소를 포함합니다. 예를 들어 이 구성 파일은 다음을 제외한 엔터프라이즈용 Microsoft 365 앱 모든 Publisher.
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Office 배포 도구 개요](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

