---
title: ADFS 페더레이션 인증서 만료
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952975"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS 페더레이션 인증서 만료

이 문제를 해결하기 위해 다음 단계를 수행합니다.
  
1. 컴퓨터에 Microsoft Azure Active Directory 모듈을 Windows PowerShell 모듈을 설치합니다(모듈이 아직 설치되지 않은 경우). 이 작업을 위해 에서 를 사용하여 [Azure AD Windows PowerShell.](https://aka.ms/aadposh)

2. 페더러가 Microsoft 365, Azure 또는 Intune에 로그인할 때 AD [FS에서 "사이트에](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)액세스하는 데 문제가 발생했습니다." 오류의 "시나리오 1: AD FS 토큰 서명 인증서 만료" 섹션의 단계를 따릅니다.

3. Microsoft, Azure 또는 [Intune에서](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)페더니트 도메인 설정 업데이트 또는 복구의 단계를 따릅니다.

    페더링 인증서 갱신에 대한 자세한 내용은 [Renew federation certificates for Microsoft 365 and Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
