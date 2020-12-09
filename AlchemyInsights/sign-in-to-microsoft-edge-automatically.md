---
title: Microsoft Edge에 자동으로 로그인
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599499"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="1010d-102">Microsoft Edge에 자동으로 로그인</span><span class="sxs-lookup"><span data-stu-id="1010d-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="1010d-103">Microsoft Edge는 OS의 기본 계정을 사용하여 사용자의 장치가 구성된 방식에 따라 자동으로 사용자에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="1010d-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="1010d-104">각 장치 구성 유형 및 해당 종속 사용자 로그인 프로세스의 시나리오는 아래에서 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="1010d-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="1010d-105">**디바이스가 하이브리드/AAD-J:** 이 옵션은 Windows 10, 다운 수준 Windows 및 해당 서버 버전에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1010d-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="1010d-106">사용자는 Azure AD(Active Directory) 계정으로 자동으로 로그인됩니다.</span><span class="sxs-lookup"><span data-stu-id="1010d-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="1010d-107">**디바이스가 도메인에** 가입된 경우: 이 옵션은 Windows 10, 다운 수준 Windows 및 해당 서버 버전에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1010d-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="1010d-108">기본적으로 도메인 계정이 있는 사용자는 자동으로 로그인되지 않습니다. 자동 로그인을 사용하도록 설정하려면 **ConfigureOnPremisesAccountAutoSignIn 정책을** 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="1010d-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="1010d-109">Azure AD 계정이 있는 사용자에 대해 자동 로그인을 사용하도록 설정하려면 디바이스를 하이브리드에 가입하는 것을 고려하세요.</span><span class="sxs-lookup"><span data-stu-id="1010d-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="1010d-110">**OS의** 기본 계정은 Microsoft 계정입니다. 이 옵션은 Windows 10 RS3(버전 1709, 빌드 10.0.16299) 이상 버전에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1010d-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="1010d-111">이 시나리오는 엔터프라이즈 장치에서는 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1010d-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="1010d-112">그러나 OS의 기본 계정이 Microsoft 계정인 경우 Microsoft Edge는 Microsoft 계정을 통해 사용자를 자동으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="1010d-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
