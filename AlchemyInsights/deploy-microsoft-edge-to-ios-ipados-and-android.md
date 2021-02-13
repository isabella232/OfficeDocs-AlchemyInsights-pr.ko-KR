---
title: iOS, iPadOS 및 Android에 Microsoft Edge 배포
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50178003"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="279b1-102">iOS, iPadOS 및 Android에 Microsoft Edge 배포</span><span class="sxs-lookup"><span data-stu-id="279b1-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="279b1-103">아래 요약된 안내 시나리오는 iOS, iPadOS 및 Android 장치의 사용자에게 Microsoft Edge를 할당하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="279b1-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="279b1-104">사용자가 모바일 장치 등록을 차단한 경우 이 안내된 시나리오는 작동하지 않습니다. 사용자가 직접 Microsoft Edge를 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="279b1-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="279b1-105">안내된 시나리오에는 다음 단계가 관련됩니다.</span><span class="sxs-lookup"><span data-stu-id="279b1-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="279b1-106">필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="279b1-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="279b1-107">소개</span><span class="sxs-lookup"><span data-stu-id="279b1-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="279b1-108">기본 사항</span><span class="sxs-lookup"><span data-stu-id="279b1-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="279b1-109">구성</span><span class="sxs-lookup"><span data-stu-id="279b1-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="279b1-110">할당</span><span class="sxs-lookup"><span data-stu-id="279b1-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="279b1-111">검토 및 만들기</span><span class="sxs-lookup"><span data-stu-id="279b1-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="279b1-112">안내 시나리오의 단계를 완료한 후 Microsoft Intune 정책에서 비즈니스용 Microsoft Edge의 다음 기능을 사용하도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="279b1-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="279b1-113">이중 ID</span><span class="sxs-lookup"><span data-stu-id="279b1-113">Dual identity</span></span>
- <span data-ttu-id="279b1-114">Microsoft Intune 앱 보호 정책과 통합</span><span class="sxs-lookup"><span data-stu-id="279b1-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="279b1-115">Azure Active Directory 응용 프로그램 프록시와 통합</span><span class="sxs-lookup"><span data-stu-id="279b1-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="279b1-116">관리되는 즐겨찾기 및 홈페이지 바로 가기</span><span class="sxs-lookup"><span data-stu-id="279b1-116">Managed favorites and home page shortcuts</span></span>
