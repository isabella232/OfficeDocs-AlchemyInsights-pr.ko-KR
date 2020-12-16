---
title: 전송 서비스 - 모든 RDFE 서비스를 다른 구독으로 이동
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681478"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="07ee9-102">전송 서비스 - 모든 RDFE 서비스를 다른 구독으로 이동</span><span class="sxs-lookup"><span data-stu-id="07ee9-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="07ee9-103">**자원 이동**</span><span class="sxs-lookup"><span data-stu-id="07ee9-103">**Move resources**</span></span>

<span data-ttu-id="07ee9-104">Azure Portal, Azure PowerShell, Azure CLI 또는 REST API를 사용하여 동일한 구독의 다른 Azure 구독 또는 리소스 그룹으로 Azure 리소스를 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="07ee9-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="07ee9-105">리소스를 이동하기 전에 다음을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="07ee9-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="07ee9-106">자원 이동 전 검사 목록</span><span class="sxs-lookup"><span data-stu-id="07ee9-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="07ee9-107">이동할 수 있는 서비스</span><span class="sxs-lookup"><span data-stu-id="07ee9-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="07ee9-108">이동의 유효성을 검사하는 방법</span><span class="sxs-lookup"><span data-stu-id="07ee9-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="07ee9-109">서비스에 대한 이동 지침</span><span class="sxs-lookup"><span data-stu-id="07ee9-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="07ee9-110">기존 리소스를 다른 리소스 그룹 또는 구독으로 이동하려면 다음을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="07ee9-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="07ee9-111">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="07ee9-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="07ee9-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="07ee9-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="07ee9-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="07ee9-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="07ee9-114">REST API</span><span class="sxs-lookup"><span data-stu-id="07ee9-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="07ee9-115">자습서: Azure 리소스를 다른 리소스 그룹 또는 [구독으로 이동](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="07ee9-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="07ee9-116">**Azure Resource Manager를 사용하여 오류 해결**</span><span class="sxs-lookup"><span data-stu-id="07ee9-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="07ee9-117">아래의 문서를 참조하여 몇 가지 일반적인 Azure 배포 오류에 대해 알아보고 문제를 해결하기 위한 정보를 받으세요.</span><span class="sxs-lookup"><span data-stu-id="07ee9-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="07ee9-118">배포 오류에 대한 오류 코드를 찾을 수 없는 경우 오류 [코드 찾기를 참조합니다.](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)</span><span class="sxs-lookup"><span data-stu-id="07ee9-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="07ee9-119">배포 오류 해결</span><span class="sxs-lookup"><span data-stu-id="07ee9-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="07ee9-120">Azure 리소스를 새 리소스 그룹 또는 구독으로 이동하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="07ee9-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="07ee9-121">무료에서 유료로 전환하는 등 Azure 구독을 업그레이드하려면 구독을 변환해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="07ee9-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="07ee9-122">무료 평가판을 업그레이드하려면 무료 평가판 업그레이드 또는 Microsoft Azure 구독을 유료로 업그레이드를 [참조하세요.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="07ee9-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="07ee9-123">유료 계정을 변경하려면 [Azure Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)구독을 다른 제품으로 변경하세요.</span><span class="sxs-lookup"><span data-stu-id="07ee9-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="07ee9-124">**Azure 구독을 추가하거나 Azure Active Directory 테넌트에 연결하려면**</span><span class="sxs-lookup"><span data-stu-id="07ee9-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="07ee9-125">로그인하고 Azure Portal의 구독 페이지에서 사용할 [구독을 선택합니다.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)</span><span class="sxs-lookup"><span data-stu-id="07ee9-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="07ee9-126">디렉터리 **변경을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="07ee9-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="07ee9-127">나타나는 경고를 검토한 다음 변경을 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="07ee9-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="07ee9-128">구독에 대한 디렉터리가 변경된 경우 성공 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="07ee9-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="07ee9-129">디렉터리 *전환을* 사용하여 새 디렉터리로 이동하십시오.</span><span class="sxs-lookup"><span data-stu-id="07ee9-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="07ee9-130">모든 것이 제대로 표시될 때 최대 10분이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="07ee9-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="07ee9-131">**권장 문서**</span><span class="sxs-lookup"><span data-stu-id="07ee9-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="07ee9-132">Azure 구독 소유권 이전</span><span class="sxs-lookup"><span data-stu-id="07ee9-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="07ee9-133">자원을 새 리소스 그룹 또는 구독으로 이동</span><span class="sxs-lookup"><span data-stu-id="07ee9-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="07ee9-134">Azure Portal을 사용하여 리소스 관리</span><span class="sxs-lookup"><span data-stu-id="07ee9-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
