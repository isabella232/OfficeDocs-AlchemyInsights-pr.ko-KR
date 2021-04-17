---
title: AIP 클라이언트에서 자동 분류가 예상대로 작동하지 않음
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
- "9002266"
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820904"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a><span data-ttu-id="3bfe8-102">AIP 클라이언트에서 자동 분류가 예상대로 작동하지 않음</span><span class="sxs-lookup"><span data-stu-id="3bfe8-102">Automatic classification not behaving as expected with the AIP client</span></span>

<span data-ttu-id="3bfe8-103">자동 분류가 예상대로 작동하지 않는 경우 다음 권장 지침을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-103">Automatic classification not behaving as expected, use the following recommended guidelines:</span></span>

1. <span data-ttu-id="3bfe8-104">자동 레이블 지정에 문제가 있는 경우 [Azure Information Protection에 대한 자동 및 권장 분류 조건을 구성하는 방법](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) 및 [중요한 정보 유형이 찾는 항목](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-104">If you are having issues with automatic labeling, see [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
2. <span data-ttu-id="3bfe8-105">올바르게 구성되지 않은 범위 지정 정책을 사용 중인지 확인합니다. [범위 지정된 정책을 사용하여 특정 사용자에 대한 Azure Information Protection 정책을 구성하는 방법](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-105">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
3. <span data-ttu-id="3bfe8-106">레이블이 지정된 문서를 연결할 때 Outlook에서 자동 레이블 지정이 작동하지 않는 경우 여기에 설명된 것과 같이 `DRMEncryptProperty`이(가) 정의되어 있지 않은지 확인합니다. [보안용 IRM 레지스트리 설정](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="3bfe8-106">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that `DRMEncryptProperty` isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>
4. <span data-ttu-id="3bfe8-107">Azure Information Protection 정책의 [기본 제공 정보 유형](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b)을 사용한 경우 콘텐츠가 예상한 형식과 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-107">If you used the [built-in information types](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) for your Azure Information Protection policy, verify that your content matches the expected format.</span></span>
5. <span data-ttu-id="3bfe8-108">레이블이 **자동** 또는 **권장** 설정에 맞게 적절히 구성되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-108">Verify that the label is appropriately configured for **Automatic** or **Recommended**.</span></span> <span data-ttu-id="3bfe8-109">**자동** 레이블 지정은 모든 Microsoft 365 앱에서 사용할 수 있지만, **권장** 설정은 Outlook을 제외한 모든 Microsoft 365 앱에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-109">(**Automatic** labeling is available for all Microsoft 365 apps, whereas **Recommended** is available for all Microsoft 365 apps except for Outlook.)</span></span>
6. <span data-ttu-id="3bfe8-110">이전에 수동으로 레이블을 지정했거나, 이전에 상위 분류로 레이블이 자동으로 지정된 문서 및 전자 메일에는 자동 분류를 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-110">You cannot use automatic classification for documents and emails that were previously manually labeled or previously automatically labeled with a higher classification.</span></span>  <span data-ttu-id="3bfe8-111">자세한 내용은 [자동 또는 권장 레이블이 적용되는 방식](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-111">For more information, see: [How automatic or recommended labels are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).</span></span>
7. <span data-ttu-id="3bfe8-112">문제가 계속 발생하는 경우 Azure Information Protection 클라이언트 로그를 수집하고 내보낸 로그를 지원 티켓에 첨부하세요.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-112">If you are still experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to your support ticket.</span></span> <span data-ttu-id="3bfe8-113">Azure Information Protection 로그를 내보내려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-113">To export Azure Information Protection logs:</span></span>
    - <span data-ttu-id="3bfe8-114">Office 문서를 열거나 Outlook에서 새 전자 메일을 작성합니다.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-114">Open an Office document or create a new email in Outlook.</span></span>
    - <span data-ttu-id="3bfe8-115">**보호/민감도** > **도움말 및 피드백** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-115">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
    - <span data-ttu-id="3bfe8-116">**로그 내보내기** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-116">Click **Export Logs**.</span></span>
    - <span data-ttu-id="3bfe8-117">원하는 위치에 로그를 저장하고 서비스 요청에 첨부합니다.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-117">Save the logs to your choice of location, and attach them to your service request.</span></span>

<span data-ttu-id="3bfe8-118">자세한 내용은 다음 항목을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="3bfe8-118">For additional information, see:</span></span>

- [<span data-ttu-id="3bfe8-119">Azure Information Protection에 대한 자동 및 권장 분류 조건을 구성하는 방법</span><span class="sxs-lookup"><span data-stu-id="3bfe8-119">How to configure conditions for automatic and recommended classification for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [<span data-ttu-id="3bfe8-120">Azure Information Protection을 사용하는 일반적인 시나리오에 대한 방법 가이드</span><span class="sxs-lookup"><span data-stu-id="3bfe8-120">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [<span data-ttu-id="3bfe8-121">Azure Information Protection 설명서 검토</span><span class="sxs-lookup"><span data-stu-id="3bfe8-121">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="3bfe8-122">Azure Information Protection 구독 및 기능 검토</span><span class="sxs-lookup"><span data-stu-id="3bfe8-122">Review Azure Information Protection subscriptions and features</span></span>](https://azure.microsoft.com/pricing/details/information-protection)
- [<span data-ttu-id="3bfe8-123">Azure Information Protection에 대한 요구 사항</span><span class="sxs-lookup"><span data-stu-id="3bfe8-123">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="3bfe8-124">Azure Information Protection에 대한 빠른 시작 튜토리얼</span><span class="sxs-lookup"><span data-stu-id="3bfe8-124">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="3bfe8-125">Azure Information Protection 클라이언트 다운로드</span><span class="sxs-lookup"><span data-stu-id="3bfe8-125">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
