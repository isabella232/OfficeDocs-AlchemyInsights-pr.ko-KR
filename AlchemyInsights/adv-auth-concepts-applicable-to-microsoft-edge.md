---
title: Microsoft Edge에 적용할 수 있는 고급 인증 개념
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398591"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="1ef74-102">Microsoft Edge에 적용할 수 있는 고급 인증 개념</span><span class="sxs-lookup"><span data-stu-id="1ef74-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="1ef74-103">다음은 Microsoft Edge에 적용되는 고급 인증 개념입니다.</span><span class="sxs-lookup"><span data-stu-id="1ef74-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="1ef74-104">**사전 인증**</span><span class="sxs-lookup"><span data-stu-id="1ef74-104">**Proactive Authentication**</span></span>

<span data-ttu-id="1ef74-105">[ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) 정책을 사용하도록 설정하면 Microsoft Edge는 Microsoft 서비스를 통해 로그인한 사용자를 사전 인증하려고 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef74-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="1ef74-106">정기적으로 온라인 서비스를 사용하여 사전 인증을 관리하는 구성이 포함된 업데이트된 매니페스트를 검사합니다.</span><span class="sxs-lookup"><span data-stu-id="1ef74-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="1ef74-107">이점: 사전 인증을 사용하면 Office 새 탭 페이지와 같은 주요 서비스에 대한 인증을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef74-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="1ef74-108">또한 Bing이 검색 엔진으로 사용되는 경우 사전 인증을 사용하면 주소 표시줄의 성능이 향상될 수 있으며 비즈니스 요구에 맞게 개인 설정된 검색 결과를 생성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef74-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="1ef74-109">**NTLM 인증용 Windows Hello CredUI**</span><span class="sxs-lookup"><span data-stu-id="1ef74-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="1ef74-110">웹 사이트에서 NTLM 또는 협상 메커니즘을 통해 사용자에 로그인할 때 SSO(Single Sign-On)를 사용할 수 없는 경우 이 기능을 사용하면 사용자가 웹 사이트와 OS 자격 증명을 공유하고 Windows Hello Cred UI를 사용하여 인증 과제를 충족할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef74-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="1ef74-111">이 로그인 흐름은 Windows 10에서만 나타나며 NTLM 또는 협상 챌린지 중에 SSO를 얻지 않은 사용자만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="1ef74-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="1ef74-112">**저장된 암호를 사용하여 자동으로 로그인**</span><span class="sxs-lookup"><span data-stu-id="1ef74-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="1ef74-113">Microsoft Edge에서 암호를 저장하는 사용자는 자격 증명을 저장한 웹 사이트에 대한 자동 로그인을 사용하도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef74-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="1ef74-114">사용자는 이 기능을 설정하거나 해제할 수 edge://settings/passwords 암호 관리자 정책에서 [구성할 수](https://go.microsoft.com/fwlink/?linkid=2134622) 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1ef74-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
