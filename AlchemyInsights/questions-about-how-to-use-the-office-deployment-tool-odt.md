---
title: ODT (Office 배포 도구)를 사용 하는 방법에 대 한 질문
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774897"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="3e838-102">ODT (Office 배포 도구)를 사용 하는 방법에 대 한 질문</span><span class="sxs-lookup"><span data-stu-id="3e838-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="3e838-103">Office 배포 도구를 [Microsoft 다운로드 센터](https://go.microsoft.com/fwlink/p/?LinkID=626065)에서 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="3e838-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="3e838-104">파일을 다운로드한 후에 Office 배포 도구 실행 파일(setup.exe) 및 샘플 구성 파일(configuration.xml)이 포함된 자동 압축 풀기 실행 파일을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="3e838-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="3e838-105">**클라이언트 컴퓨터에서 엔터프라이즈 제품에 대 한 Microsoft 365 앱을 제외 하거나 제거 하려면:**</span><span class="sxs-lookup"><span data-stu-id="3e838-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="3e838-106">Enterprise 용 Microsoft 365 앱을 설치할 때 특정 제품을 제외할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3e838-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="3e838-107">이렇게 하려면 ODT를 사용하여 Office를 설치하기 위한 단계를 수행하되 구성 파일에 ExcludeApp 요소를 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="3e838-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="3e838-108">예를 들어이 구성 파일은 Publisher를 제외한 모든 Microsoft 365 앱 (enterprise 제품)을 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="3e838-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="3e838-109">Office 배포 도구 개요</span><span class="sxs-lookup"><span data-stu-id="3e838-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

