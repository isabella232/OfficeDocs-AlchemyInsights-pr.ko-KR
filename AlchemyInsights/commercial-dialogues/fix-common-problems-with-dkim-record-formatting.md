---
title: DKIM 레코드 서식의 일반적인 문제 해결
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737865"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="50509-102">DKIM 레코드 서식의 일반적인 문제 해결</span><span class="sxs-lookup"><span data-stu-id="50509-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="50509-103">대부분의 DKIM 설정 문제는 잘못된 DNS 레코드와 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="50509-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="50509-104">DKIM 설정 문제를 해결하려면 DKIM CNAME 레코드(TXT 레코드 아님)의 서식이 올바르게 지정되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="50509-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="50509-105">자세한 내용은 [Office 365에서 DKIM을](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)수동으로 설정하기 위해 필요한 작업을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="50509-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="50509-106">일반적으로 DNS 레코드에 대한 도움이 필요한 경우 [Office 365용 DNS](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)호스팅 공급자에서 DNS 레코드 만들기를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="50509-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="50509-107">도메인의 DNS 호스팅 서비스에서 DKIM DNS 레코드를 만들거나 업데이트한 후 DNS 레코드가 전파될 때까지 기다려야 합니다.</span><span class="sxs-lookup"><span data-stu-id="50509-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
