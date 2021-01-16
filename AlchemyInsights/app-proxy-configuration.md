---
title: 앱 프록시 구성
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876560"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="1f93a-102">앱 프록시 구성</span><span class="sxs-lookup"><span data-stu-id="1f93a-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="1f93a-103">클라우드에 대한 응용 프로그램 프록시 응용 프로그램을 표시하도록 Azure AD 내에서 응용 프로그램 프록시 응용 프로그램을 구성하는 방법을 이해하기 위해 응용 프로그램 프록시 응용 프로그램을 구성하는 [방법을 참조하세요.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)</span><span class="sxs-lookup"><span data-stu-id="1f93a-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="1f93a-104">SSO(Single Sign-On)를 사용하면 사용자가 여러 번 인증하지 않고도 응용 프로그램에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1f93a-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="1f93a-105">단일 인증이 클라우드, Azure Active Directory에 대해 실행될 수 있도록 허용하고 서비스 또는 커넥터가 사용자로 가장하여 응용 프로그램에서 추가 인증 과제를 완료할 수 있도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="1f93a-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="1f93a-106">자세한 내용은 응용 프로그램 프록시 응용 프로그램에 [대한 Single Sign-On을 구성하는 방법을 참조합니다.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)</span><span class="sxs-lookup"><span data-stu-id="1f93a-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="1f93a-107">이 [문서를 사용하여](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) 새 응용 프로그램 프록시 응용 프로그램을 만들 때 사용자가 직면하는 일반적인 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1f93a-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="1f93a-108">응용 프로그램에 대한 백 엔드 인증을 설정하는 데 문제가 있는 경우 응용 프로그램 프록시에 [대한 Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) 제한 위임 구성을 해결하거나 [PingAccess를](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) 사용하여 응용 프로그램을 구성하여 문제를 해결해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1f93a-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
