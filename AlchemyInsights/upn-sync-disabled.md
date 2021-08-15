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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038118"
---
# <a name="upn-sync-disabled"></a>UPN 동기화를 사용하지 않도록 설정

2016년 3월 30일 전에 Azure AD와 동기화를 시작한 경우 다음 Azure AD PowerShell cmdlet을 실행하여 조직에 대한 UPN 소프트 일치만 사용하도록 설정하세요.
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN 소프트 일치는 2016년 3월 30일 또는 그 이후에 Azure AD와 동기화를 시작한 조직에 대해 자동으로 설정됩니다.
  
UPN 및 기타 동기화 기능에서 소프트 일치를 사용하도록 설정하는 데 대한 자세한 내용은 Azure AD 커넥트 [동기화 서비스 기능을 참조하세요.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

