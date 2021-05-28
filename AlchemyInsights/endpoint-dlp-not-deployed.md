---
title: 엔드포인트 DLP가 사용자의 장치에 배포되지 않음
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52694808"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="c5442-102">엔드포인트 DLP가 사용자의 장치에 배포되지 않음</span><span class="sxs-lookup"><span data-stu-id="c5442-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="c5442-103">엔드포인트 데이터 손실 방지(DLP) 설정이 사용자의 장치에 적용되지 않은 경우 다음 요구 사항을 충족하는지 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="c5442-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="c5442-104">Windows 10 x64 빌드 1809 이상이 장치에 설치되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c5442-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="c5442-105">맬웨어 방지 클라이언트 버전 4.18.2009.7 이상이 설치되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c5442-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="c5442-106">장치가 다음 중 **하나** 입니다.</span><span class="sxs-lookup"><span data-stu-id="c5442-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="c5442-107">Azure AD(Azure Active Directory) 조인됨</span><span class="sxs-lookup"><span data-stu-id="c5442-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="c5442-108">하이브리드 Azure AD 조인됨</span><span class="sxs-lookup"><span data-stu-id="c5442-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="c5442-109">AAD 등록됨</span><span class="sxs-lookup"><span data-stu-id="c5442-109">AAD registered</span></span>

- <span data-ttu-id="c5442-110">클라우드로 업로드 활동에 대한 정책 작업을 적용하려면, 엔드포인트 장치에 Microsoft Chromium Edge 브라우저를 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="c5442-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="c5442-111">Endpoint DLP 배포에 대한 추가 요구 사항은 [Endpoint 데이터 손실 방지 시작하기](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5442-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>