---
title: 규정 준수 센터에서 AIP로부터 MIP/통합 레이블로 마이그레이션
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825377"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="ca97b-102">규정 준수 센터에서 AIP로부터 MIP/통합 레이블로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="ca97b-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="ca97b-103">보안 및 규정 준수 센터에서 AIP 레이블로부터 통합 레이블로 마이그레이션하려면 다음을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="ca97b-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="ca97b-104">**Azure portal에서 보호 활성화**</span><span class="sxs-lookup"><span data-stu-id="ca97b-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="ca97b-105">아직 실행하지 않은 경우 새 브라우저 창을 열고 [Azure portal에 로그인](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)합니다.</span><span class="sxs-lookup"><span data-stu-id="ca97b-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="ca97b-106">**Azure Information Protection** 블레이드를 탐색합니다.</span><span class="sxs-lookup"><span data-stu-id="ca97b-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="ca97b-107">예를 들어 허브 메뉴에서 **모든 서비스** 를 클릭하고 필터 상자에 **정보** 를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="ca97b-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="ca97b-108">**Azure Information Protection** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ca97b-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="ca97b-109">전에 Azure Information Protection 블레이드에 액세스한 적이 없는 경우 일회성의 [추가 단계](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time)를 참조하여 포털에 블레이드를 추가하세요.</span><span class="sxs-lookup"><span data-stu-id="ca97b-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="ca97b-110">Azure Information Protection 블레이드를 열려면 [Azure Information Protection 프리미엄 플랜](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) 또는 권한 관리가 포함된 Office 365 플랜이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ca97b-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="ca97b-111">구독 중 하나를 이용하고 있지만 유효한 구독을 찾을 수 없다는 메시지가 표시되면 [Microsoft 지원에 문의](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support)하거나 기본 지원 채널을 이용하세요.</span><span class="sxs-lookup"><span data-stu-id="ca97b-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="ca97b-112">**관리** 메뉴 옵션을 찾고 **보호 활성화** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ca97b-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="ca97b-113">**활성화** 를 클릭한 후 작업을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ca97b-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="ca97b-114">활성화가 완료되면 정보 표시줄에 **활성화가 성공적으로 완료되었습니다** 라는 문구가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ca97b-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="ca97b-115">**Azure Information Protection 레이블을 Office 365 보안 및 준수 센터로 마이그레이션**</span><span class="sxs-lookup"><span data-stu-id="ca97b-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="ca97b-116">전역 관리자 권한을 가진 사용자로 로그인했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="ca97b-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="ca97b-117">**Azure Information Protection** 블레이드를 탐색합니다.</span><span class="sxs-lookup"><span data-stu-id="ca97b-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="ca97b-118">**관리** 메뉴 옵션에서 **통합 레이블** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ca97b-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="ca97b-119">**Azure Information Protection-통합 레이블** 블레이드에서 **활성화** 를 클릭하고 온라인 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="ca97b-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="ca97b-120">**참고**: 보안 및 준수 센터 마이그레이션을 활성화하기 전에 적합한 사용 권한이 있는지 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="ca97b-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="ca97b-121">자세한 내용은 다음 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ca97b-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="ca97b-122">Azure Information Protection을 구성하기 위해서는 전역 관리자가 되야 하나요? 아니면 다른 관리자에게 위임할 수 있나요?</span><span class="sxs-lookup"><span data-stu-id="ca97b-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="ca97b-123">보안 및 준수 센터로 마이그레이션한 후 관리자 역할에 대한 중요 정보</span><span class="sxs-lookup"><span data-stu-id="ca97b-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="ca97b-124">보안 및 규정 준수 센터 내 AIP에서 통합 레이블로 마이그레이션 관련하여 자세한 내용은 [레이블 마이그레이션](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels) 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ca97b-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
