---
title: GPO 배포
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417167"
---
# <a name="gpo-deployment"></a><span data-ttu-id="cc702-102">GPO 배포</span><span class="sxs-lookup"><span data-stu-id="cc702-102">GPO Deployment</span></span>

<span data-ttu-id="cc702-103">Azure AD DS(Azure Active Directory Domain Services)의 사용자 및 컴퓨터 개체에 대한 설정은 일반적으로 GPOS(그룹 정책 개체)를 사용하여 관리됩니다.</span><span class="sxs-lookup"><span data-stu-id="cc702-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="cc702-104">Azure AD DS에는 AADDC 사용자 및 AADDC 컴퓨터 컨테이너에 대한 기본 제공 GPOS가 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cc702-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="cc702-105">필요에 따라 이러한 기본 제공 GPOS를 사용자 지정하여 환경에 맞게 그룹 정책을 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cc702-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="cc702-106">Azure AD DC 관리자 그룹의 구성원은 Azure AD DS 도메인의 그룹 정책 관리 권한을 가지며 사용자 지정 GPOS 및 OUS(조직 단위)를 만들 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cc702-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="cc702-107">그룹 정책의 기능 및 작동 방식에 대한 자세한 내용은 그룹 정책 개요 [를 참조하세요.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="cc702-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="cc702-108">하이브리드 환경에서는 온-프레미스 AD DS 환경에서 구성된 그룹 정책이 Azure AD DS와 동기화되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="cc702-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="cc702-109">Azure AD DS의 사용자 또는 컴퓨터에 대한 구성 설정을 정의하려면 기본 GPO 중 하나를 편집하거나 사용자 지정 GPO를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cc702-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="cc702-110">이 [그룹 정책 관리](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) 문서는 그룹 정책 관리 도구를 설치하는 방법, 기본 제공 GOS를 편집하는 방법 및 사용자 지정 GOS를 만드는 방법을 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="cc702-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
