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
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821957"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS 페더레이션 인증서 만료

이 문제를 해결하기 위해 다음 단계를 수행합니다.
  
1. 컴퓨터에 Microsoft Azure Active Directory 모듈을 Windows PowerShell 설치합니다(모듈이 아직 설치되지 않은 경우). 이 작업을 위해 를 사용하여 [Azure AD 관리로 Windows PowerShell.](https://aka.ms/aadposh)

2. 페더링 사용자가 [Microsoft 365, Azure 또는 Intune에](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)로그인할 때 AD FS에서 "사이트에 액세스하는 데 문제가 발생했습니다." 오류의 "시나리오 1: AD FS 토큰 서명 인증서 만료" 섹션의 단계를 따릅니다.

3. Microsoft, Azure 또는 [Intune에서](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)페더니트 도메인 설정 업데이트 또는 복구의 단계를 따릅니다.

    페더링 인증서 갱신에 대한 자세한 내용은 [Microsoft 365 및 Azure Active Directory에 대한 페더링 인증서 갱신을 참조하세요.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
