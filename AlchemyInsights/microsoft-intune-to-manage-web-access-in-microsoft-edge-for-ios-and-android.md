---
title: Microsoft Intune을 사용하여 iOS 및 Android용 Microsoft Edge에서 웹 액세스 관리
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617282"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="ccece-102">Microsoft Intune을 사용하여 iOS 및 Android용 Microsoft Edge에서 웹 액세스 관리</span><span class="sxs-lookup"><span data-stu-id="ccece-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="ccece-103">iOS 및 Android용 Microsoft Edge를 사용하면 완전히 분리된 여러 프로필에서 웹을 탐색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ccece-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="ccece-104">Microsoft Intune 및 Azure Active Directory Premium 기능(예: 조건부 액세스)이 포함된 Enterprise Mobility + Security 제품군을 구독하면 Microsoft 365 데이터에 대한 가장 광범위한 보호 기능을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ccece-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="ccece-105">최소한 사용자가 모바일 장치에서 iOS 및 Android용 Microsoft Edge로 연결할 수 있도록 하고 (2) 보호된 검색 환경을 제공하는 Microsoft Intune 앱 보호 정책을 구현하는 조건부 액세스 정책을 배포해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ccece-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="ccece-106">조건부 액세스 및 정책을 사용하는 방법을 이해하기 위해 다음을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="ccece-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="ccece-107">Azure Active Directory 조건부 액세스 정책 적용</span><span class="sxs-lookup"><span data-stu-id="ccece-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="ccece-108">Microsoft Intune 앱 보호 정책 만들기</span><span class="sxs-lookup"><span data-stu-id="ccece-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="ccece-109">정책으로 보호된 브라우저에서 Azure Active Directory 연결 웹앱에 Single Sign-On 사용</span><span class="sxs-lookup"><span data-stu-id="ccece-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="ccece-110">앱 구성을 사용하여 검색 환경 관리</span><span class="sxs-lookup"><span data-stu-id="ccece-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="ccece-111">직장 및 학교 계정만 사용할 수 있도록 허용</span><span class="sxs-lookup"><span data-stu-id="ccece-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="ccece-112">일반 앱 구성 정책 배포</span><span class="sxs-lookup"><span data-stu-id="ccece-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="ccece-113">데이터 보호를 위한 앱 구성 정책 배포</span><span class="sxs-lookup"><span data-stu-id="ccece-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="ccece-114">Microsoft Endpoint Manager를 사용하여 앱 구성 정책 배포</span><span class="sxs-lookup"><span data-stu-id="ccece-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="ccece-115">관리되는 앱 로그에 액세스하는 방법에 대한 자세한 내용은 iOS 및 [Android용 Microsoft Edge를](https://go.microsoft.com/fwlink/?linkid=2132578)사용하여 관리되는 앱 로그에 액세스합니다.</span><span class="sxs-lookup"><span data-stu-id="ccece-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
