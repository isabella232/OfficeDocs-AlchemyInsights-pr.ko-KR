---
title: 조직 전체 주소 목록 및 오프라인 주소록 관리
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
- "9002895"
- "5550"
ms.openlocfilehash: a15864f34433695b61ea040abd3032d234920653
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812697"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="8d95a-102">조직 전체 주소 목록(GAL) 및 오프라인 주소록 관리(OAB)</span><span class="sxs-lookup"><span data-stu-id="8d95a-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="8d95a-103">전체 주소 목록(GAL)은 조직에서 메일 사용이 가능한 개체(전자 메일을 받을 수 있는 모든 받는 사람 유형)의 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="8d95a-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="8d95a-104">모든 조직에서 GAL은 자동으로 생성됩니다.</span><span class="sxs-lookup"><span data-stu-id="8d95a-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="8d95a-105">조직이나 위치별로 사용자를 구분할 추가 GAL를 만들 수 있지만, 단일 사용자는 한 번에 하나의 GAL만 보고 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8d95a-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="8d95a-106">Windows용 Outlook과 같은 일부 전자 메일 클라이언트는 오프라인 사용을 위해 GAL을 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="8d95a-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="8d95a-107">이를 오프라인 주소록(OAB)이라고 합니다.</span><span class="sxs-lookup"><span data-stu-id="8d95a-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="8d95a-108">Exchange online에서 OAB는 8시간 마다 한 번만 업데이트되고 그 후 클라이언트는 이를 다운로드하여 로컬 OAB 복사본을 업데이트해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8d95a-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="8d95a-109">모든 받는 사람에 대한 변경 내용은 먼저 GAL에서 확인되어야 하고 이후에 OAB에서 확인할 수 있도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="8d95a-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="8d95a-110">일반적으로 사용되는 GAL과 OAB 절차는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="8d95a-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="8d95a-111">다양한 이유로 GAL에서 일부 개체를 숨기는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="8d95a-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="8d95a-112">[주소 목록에서 받는 사람 숨기기](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8d95a-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="8d95a-113">특정 사용자 그룹에 조직의 GAL에 대한 사용자 지정 보기를 제공해야 하는 경우에는 [Exchange Online에서의 주소록 정책](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8d95a-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="8d95a-114">[Exchange Online에서 전체 주소 목록 만들기](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list)를 수행하고 GAL 사용 권한을 작업하는 방법에 대한 내용은 [Exchange Online에서의 주소 목록](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8d95a-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="8d95a-115">새 GAL을 만드는 경우 새 OAB를 만드는 것이 좋을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8d95a-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="8d95a-116">[오프라인 주소록 절차](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8d95a-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
