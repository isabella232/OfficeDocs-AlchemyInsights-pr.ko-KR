---
title: Office 365에서 구입했거나 관리되는 도메인으로 Wix 웹 사이트 사용
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
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825953"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a><span data-ttu-id="0fde6-102">Office 365에서 구입했거나 관리되는 도메인으로 Wix 웹 사이트 사용</span><span class="sxs-lookup"><span data-stu-id="0fde6-102">Using Wix website with Office 365 purchased or managed domains</span></span>

- [<span data-ttu-id="0fde6-103">DNS 레코드를 업데이트하여 현재 호스팅 공급자에 웹 사이트 유지</span><span class="sxs-lookup"><span data-stu-id="0fde6-103">Update DNS records to keep your website with your current hosting provider</span></span>](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- <span data-ttu-id="0fde6-104">Wix 문서 "포인팅 방법을 사용하여 Wix에 도메인 연결"에서는 Office 365를 사용할 때 네임 서버를 변경하는 대신 포인팅(위 링크당 DNS 레코드 추가)을 사용할 것을 권장합니다.</span><span class="sxs-lookup"><span data-stu-id="0fde6-104">Wix article "Connecting a Domain to Wix Using the Pointing Method" recommends using pointing (adding DNS records per the above link) rather than changing names servers when using Office 365</span></span>
- <span data-ttu-id="0fde6-105">그럼에도 불구하고 이름 서버를 Wix로 변경하려면 [Microsoft용 Wix에서 DNS 레코드를 생성](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0fde6-105">If you still choose to change name servers to Wix you will then need to  [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)</span></span>
- <span data-ttu-id="0fde6-106">Microsoft에서 사용자의 도메인을 구입한 경우 이름 서버를 변경할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0fde6-106">If your domain was purchased from Microsoft the name servers cannot be changed.</span></span> <span data-ttu-id="0fde6-107">이름 서버를 변경해야 하는 경우 Microsoft에서 구입한 도메인을 [60일 후에 다른 호스팅 공급자로 이전](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)해야 할 것입니다.</span><span class="sxs-lookup"><span data-stu-id="0fde6-107">If you have to change names servers the Microsoft purchased domain would need to be  [transferred to another hosting provider after 60 days](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)</span></span>