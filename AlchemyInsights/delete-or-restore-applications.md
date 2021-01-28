---
title: 응용 프로그램 삭제 또는 복원
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013985"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="e3b71-102">응용 프로그램 삭제 또는 복원</span><span class="sxs-lookup"><span data-stu-id="e3b71-102">Delete or restore applications</span></span>

<span data-ttu-id="e3b71-103">**Azure AD 테넌트에서 응용 프로그램을 삭제하려면**</span><span class="sxs-lookup"><span data-stu-id="e3b71-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="e3b71-104">Azure **AD 포털에서** 엔터프라이즈 응용 **프로그램을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="e3b71-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="e3b71-105">그런 다음 삭제할 응용 프로그램을 찾아 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e3b71-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="e3b71-106">왼쪽 **창의** 관리 섹션에서 속성을 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="e3b71-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="e3b71-107">**삭제를** 선택한 다음 **예를** 선택하여 Azure AD 테넌트에서 앱을 삭제하려는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e3b71-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="e3b71-108">앱을 삭제하는 방법에 대한 자세한 내용은 [빠른 시작: Azure AD(Azure Active Directory)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)테넌트에서 응용 프로그램 삭제를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e3b71-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="e3b71-109">PowerShell에서 [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet은 Azure Active Directory의 특정 응용 프로그램에서 응용 프로그램 프록시 구성을 제거하고 지정된 경우 응용 프로그램을 완전히 삭제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e3b71-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="e3b71-110">PowerShell을 **사용하여 삭제된 응용** 프로그램을 복원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e3b71-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="e3b71-111">복원할 응용 프로그램이 식별되면 [Restore-AzureADDeletedApplication을](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)사용하여 복원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e3b71-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
