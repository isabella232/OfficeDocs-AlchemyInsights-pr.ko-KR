---
title: DKIM 설정 문제 해결
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744956"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="a1218-102">DKIM 설정 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a1218-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="a1218-103">사용자 지정 도메인에 대해 DKIM을 사용 하도록 설정 하는 데 문제가 발생 하면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="a1218-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="a1218-104">대부분의 DKIM 설정 문제는 잘못 된 DNS 레코드와 관련이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a1218-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="a1218-105">TXT 레코드가**아닌** DKIM CNAME 레코드의 서식이 올바르게 지정 되었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a1218-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="a1218-106">자세한 내용은이 [항목](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="a1218-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="a1218-107">도메인의 DNS 호스팅 서비스 (대개 도메인 등록자)에서 DKIM DNS 레코드를 만들거나 업데이트 한 후에는 DNS 레코드가 전파 될 때까지 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="a1218-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="a1218-108">관리 센터에서 DKIM DNS 레코드를 만들 수 없는 경우 \<CustomDomain\> 사용자 지정 도메인 (예: contoso.com)으로 대체 하 여 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)에서이 명령을 실행할 수 `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a1218-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
