---
title: 도메인에 조인된 장치에서 Microsoft Edge를 기본 브라우저로 설정
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426837"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="4b3a5-102">도메인에 조인된 장치에서 Microsoft Edge를 기본 브라우저로 설정</span><span class="sxs-lookup"><span data-stu-id="4b3a5-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="4b3a5-103">Microsoft Edge를 기본 브라우저로 설정:</span><span class="sxs-lookup"><span data-stu-id="4b3a5-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="4b3a5-104">[기본 연결 구성 파일을 만들어](https://go.microsoft.com/fwlink/?linkid=2132437) 로컬 또는 네트워크 공유에 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="4b3a5-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="4b3a5-105">그룹 정책 편집기를 열어 **컴퓨터 구성** > **관리 서식 파일** > **Windows 컴포넌트** > **파일 탐색기** 로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="4b3a5-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="4b3a5-106">**기본 연결 구성 파일 설정** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="4b3a5-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="4b3a5-107">**정책 설정** 을 선택하고 **사용** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="4b3a5-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="4b3a5-108">**옵션** 에서 기본 연결 구성 파일 위치를 입력하고 **확인** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="4b3a5-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
