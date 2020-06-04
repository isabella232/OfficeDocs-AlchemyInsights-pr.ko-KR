---
title: 원활한 SSO를 사용 하도록 설정 하는 방법
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 3cf751bc42322067c4b7cd9b5facb933430f2b87
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36663872"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="47448-102">원활한 SSO를 사용 하도록 설정 하는 방법</span><span class="sxs-lookup"><span data-stu-id="47448-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="47448-103">[AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)를 통해 원활한 SSO를 사용 하도록 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="47448-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="47448-104">Azure AD Connect를 새로 설치 하는 경우에는 [사용자 지정 설치 경로](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47448-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="47448-105">**사용자 로그인** 페이지에서 **single sign-on 사용** 옵션을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47448-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="47448-106">원활한 SSO를 올바르게 사용 하도록 설정 했는지 확인 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="47448-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="47448-107">글로벌 관리자로 [Azure Active Directory 관리 센터](https://aad.portal.azure.com) 에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="47448-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="47448-108">왼쪽 창에서 **Azure Active Directory** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47448-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="47448-109">원활한 sso (single sign-on)가 **사용 하도록 설정**되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="47448-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="47448-110">자세한 내용은 [Azure Active Directory 원활한 Single sign-on: 빠른 시작](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="47448-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  