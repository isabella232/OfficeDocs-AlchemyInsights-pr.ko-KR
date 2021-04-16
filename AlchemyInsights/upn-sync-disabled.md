---
title: UPN 동기화를 사용하지 않도록 설정
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782157"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="be910-102">UPN 동기화를 사용하지 않도록 설정</span><span class="sxs-lookup"><span data-stu-id="be910-102">UPN sync disabled</span></span>

<span data-ttu-id="be910-103">2016년 3월 30일 전에 Azure AD와 동기화를 시작한 경우 다음 Azure AD PowerShell cmdlet을 실행하여 조직에 대한 UPN 소프트 일치만 사용하도록 설정하세요.</span><span class="sxs-lookup"><span data-stu-id="be910-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="be910-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="be910-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="be910-105">UPN 소프트 일치는 2016년 3월 30일 또는 그 이후에 Azure AD와 동기화를 시작한 조직에 대해 자동으로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="be910-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="be910-106">UPN 및 기타 동기화 기능에서 소프트 매치 사용에 대한 자세한 내용은 Azure AD Connect 동기화 서비스 [기능을 참조하세요.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)</span><span class="sxs-lookup"><span data-stu-id="be910-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

