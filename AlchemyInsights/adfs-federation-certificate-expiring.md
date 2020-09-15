---
title: ADFS 페더레이션 인증서 만료
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686720"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS 페더레이션 인증서 만료

이 문제를 해결 하려면 다음 단계를 수행 합니다.
  
1. 컴퓨터에 Windows PowerShell 용 Microsoft Azure Active Directory 모듈 (모듈을 아직 설치 하지 않은 경우)을 설치 합니다. 이렇게 하려면 [Windows PowerShell을 사용 하 여 AZURE AD 관리](https://aka.ms/aadposh)로 이동 합니다.

2. [페더레이션 사용자가 Microsoft 365, Azure 또는 Intune에 로그인 하는 경우 AD fs에서](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)"시나리오 1: ad FS 토큰 서명 인증서가 만료 되었습니다." 섹션의 단계를 수행 합니다.

3. [Microsoft, Azure 또는 Intune의 페더레이션 도메인 설정 업데이트 또는 복구](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)의 단계를 수행 합니다.

    페더레이션 인증서를 갱신 하는 방법에 대 한 자세한 내용은 [갱신이 federation certificate For Microsoft 365 및 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)를 참조 하십시오.
