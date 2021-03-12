---
title: 암호 정책
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718205"
---
# <a name="password-policies"></a><span data-ttu-id="f7726-102">암호 정책</span><span class="sxs-lookup"><span data-stu-id="f7726-102">Password policies</span></span>

<span data-ttu-id="f7726-103">**사용자의 암호 정책에 문제가 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="f7726-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="f7726-104">사용자의 암호 정책은 사용자가 클라우드 전용인지 아니면 사내에 있는지에 따라 결정됩니다.</span><span class="sxs-lookup"><span data-stu-id="f7726-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="f7726-105">클라우드 전용 사용자는 이 문서의 요구 사항을 충족하는 암호를 [선택해야](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts) 합니다. 클라우드 사용자 계정에만 적용되는 암호 정책</span><span class="sxs-lookup"><span data-stu-id="f7726-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="f7726-106">On-premises users must choose a password that meet the on-premises requirements.</span><span class="sxs-lookup"><span data-stu-id="f7726-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="f7726-107">프레미스 사용자가 암호를 설정할 수 없는 경우, On-premises requirements을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="f7726-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="f7726-108">**암호 만료 정책을 설정하거나 검사하는 방법을 모르는 경우**</span><span class="sxs-lookup"><span data-stu-id="f7726-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="f7726-109">PowerShell을 사용하여 테넌트의 클라우드 사용자에 대한 만료 정책을 설정하고 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f7726-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="f7726-110">이 문서의 지침에 따라 [PowerShell을](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell) 사용하여 암호 정책 설정 또는 확인</span><span class="sxs-lookup"><span data-stu-id="f7726-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="f7726-111">On-premises 사용자에 대한 암호 만료 정책은 프레미스 AD에서 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="f7726-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="f7726-112">**기타 유용한 링크:**</span><span class="sxs-lookup"><span data-stu-id="f7726-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="f7726-113">암호 재설정 시작</span><span class="sxs-lookup"><span data-stu-id="f7726-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="f7726-114">관리자가 시작한 암호 재설정 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f7726-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
