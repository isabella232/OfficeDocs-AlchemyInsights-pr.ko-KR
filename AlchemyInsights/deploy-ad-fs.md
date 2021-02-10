---
title: AD FS 배포
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50165272"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="6c197-102">AD FS 배포</span><span class="sxs-lookup"><span data-stu-id="6c197-102">Deploy AD FS</span></span>

<span data-ttu-id="6c197-103">AD FS(Active Directory Federation Services) 배포는 Office 365 서비스에 대한 사용자를 인증하는 데 사용할 수 있는 인프라를 사용하여 사용자를 인증합니다.</span><span class="sxs-lookup"><span data-stu-id="6c197-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="6c197-104">페더타 로그인을 사용하면 사용자가 Azure AD(Azure Active Directory)와 통합된 Office 365 서비스 및 SAAS(Software as a Service) 응용 프로그램에 로그인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6c197-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="6c197-105">페더러드 로그인은 AD FS를 통해 사용자의 On-프레미스 Active Directory에 대해 사용자를 인증합니다.</span><span class="sxs-lookup"><span data-stu-id="6c197-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="6c197-106">또한 회사 네트워크에서는 사용자가 암호를 다시 입력할 필요는 없습니다.</span><span class="sxs-lookup"><span data-stu-id="6c197-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="6c197-107">[AD FS](https://go.microsoft.com/fwlink/?linkid=2071178) 배포 어드바이저는 Microsoft 365 및 Office 365 서비스에 대해 사용자를 인증하는,프레미스 AD FS 인프라 배포에 대한 단계별 지침을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="6c197-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="6c197-108">이 가이드를 사용하여 조직은 AD FS 구성 요소 및 요구 사항을 검토하고, 배포에 필요한 SSL 인증서를 획득 및 설치하고, 필요한 웹 응용 프로그램 프록시 서버를 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6c197-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
