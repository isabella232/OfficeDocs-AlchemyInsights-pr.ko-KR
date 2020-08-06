---
title: Microsoft에서 구입했거나 관리되는 도메인으로 Wix 웹 사이트 사용
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/05/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5855"
- "9003096"
ms.openlocfilehash: f6845c56f05e9cef11362ce601a974b73a154c9a
ms.sourcegitcommit: 28a319e482e6a8644e87726e1b0e599819df52d0
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46572395"
---
# <a name="using-a-wix-website-with-microsoft-purchased-or-managed-domains"></a><span data-ttu-id="acad0-102">Microsoft에서 구입했거나 관리되는 도메인으로 Wix 웹 사이트 사용</span><span class="sxs-lookup"><span data-stu-id="acad0-102">Using a Wix website with Microsoft purchased or managed domains</span></span>

<span data-ttu-id="acad0-103">Microsoft에서 구입헸거나 관리되는 도메인에서 Wix 웹 사이트를 사용하는 방법에 대한 자세한 내용은 [DNS 레코드를 업데이트하여 현재 호스팅 공급자로 웹 사이트 유지](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="acad0-103">For information about how to use a Wix website with a Microsoft purchased or managed domain, see [Update DNS records to keep your website with your current hosting provider](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).</span></span>

<span data-ttu-id="acad0-104">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="acad0-104">For details, see:</span></span> 

- <span data-ttu-id="acad0-105">Wix 문서인 "Pointing Method를 사용하여 Wix에 도메인 연결"에서는 Microsoft 365를 사용할 때 이름 서버를 변경하는 대신 위의 링크에 설명된 대로 DNS 레코드를 추가하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="acad0-105">The Wix article, "Connecting a Domain to Wix Using the Pointing Method," recommends adding DNS records as outlined in the link above rather than changing names servers when you're using Microsoft 365.</span></span>

- <span data-ttu-id="acad0-106">이름 서버를 Wix로 변경하도록 선택하는 경우에는 Wix에서 Microsoft용 DNS 레코드를 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="acad0-106">If you choose to change name servers to Wix, you must create DNS records at Wix for Microsoft.</span></span> <span data-ttu-id="acad0-107">자세한 내용은 [Microsoft용 Wix에서 DNS 레코드 만들기](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="acad0-107">For more info, see [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).</span></span>

- <span data-ttu-id="acad0-108">Microsoft에서 사용자의 도메인을 구입한 경우 이름 서버를 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="acad0-108">If your domain was purchased from Microsoft the name servers can't be changed.</span></span> <span data-ttu-id="acad0-109">이름 서버를 변경해야 하는 경우 Microsoft에서 구입한 도메인을 60일 후에 다른 호스팅 공급자로 이전해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="acad0-109">If you must change names servers, the Microsoft purchased domain must be transferred to another hosting provider after 60 days.</span></span> <span data-ttu-id="acad0-110">자세한 내용은 [도메인 FAQ](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="acad0-110">For more info, see the [Domains FAQ](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).</span></span>