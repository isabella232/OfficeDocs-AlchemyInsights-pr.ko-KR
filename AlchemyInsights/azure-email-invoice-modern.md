---
title: 최신 Azure 이메일 송장 발부
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840629"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="0fb95-102">Azure에서 이메일 송장 발행</span><span class="sxs-lookup"><span data-stu-id="0fb95-102">Email invoicing in Azure</span></span>

<span data-ttu-id="0fb95-103">이메일 송장 기본 설정을 업데이트하려면 청구 프로필 또는 청구 계정의 소유자나 참가자 역할이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="0fb95-104">옵트인한 후에는 청구 프로필에서 소유자, 참가자, 독자 및 송장 관리자 역할이 있는 모든 사용자가 이메일로 송장을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="0fb95-105">[Azure 포털](https://portal.azure.com/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="0fb95-106">**비용 관리 + 청구** 검색</span><span class="sxs-lookup"><span data-stu-id="0fb95-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="0fb95-107">왼쪽에서 **송장** 을 선택한 다음, 페이지 맨 위에 있는 **이메일 송장** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="0fb95-108">청구 프로필이 여러 개인 경우에는 청구 프로필을 선택한 다음, **옵트인** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="0fb95-109">**업데이트** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-109">Select **Update**.</span></span>
6. <span data-ttu-id="0fb95-110">청구 프로필이 여러 개인 경우에는 청구 프로필을 선택한 다음, **옵트인** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="0fb95-111">다른 사용자에게 MCA 또는 MPA 청구 프로필에 대한 송장 관리자 역할을 할당하여 송장을 보고, 다운로드하고, 비용을 지불할 수 있도록 액세스 권한을 부여합니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="0fb95-112">이메일로 송장을 받도록 옵트인한 경우, 이메일로 송장을 받습니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="0fb95-113">[Azure 포털](https://portal.azure.com/)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="0fb95-114">**비용 관리 + 청구** 검색</span><span class="sxs-lookup"><span data-stu-id="0fb95-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="0fb95-115">왼쪽에서 **청구 프로필** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="0fb95-116">청구 프로필 목록에서 송장 관리자 역할을 할당하려는 청구 프로필을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="0fb95-117">왼쪽에서 **액세스 제어(IAM)** 를 선택한 다음, 페이지 맨 위에서 **추가** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="0fb95-118">역할 드롭다운 목록에서 **송장 관리자** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="0fb95-119">액세스 권한을 부여할 사용자의 이메일 주소를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="0fb95-120">**저장** 을 선택하여 역할을 할당합니다.</span><span class="sxs-lookup"><span data-stu-id="0fb95-120">Select **Save** to assign the role.</span></span>
