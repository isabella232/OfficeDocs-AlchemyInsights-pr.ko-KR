---
title: Windows Virtual Desktop에 Office 및 OneDrive 설치
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590292"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Windows Virtual Desktop에 Office 및 OneDrive 설치

1. [마스터 VHD 이미지 준비 및 사용자 지정](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). 아직 생성되지 않은 VM(가상 시스템)을 생성합니다.

1. [공유 컴퓨터 인증 모드로 Office 설치](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). 공유 컴퓨터 인증을 사용하면 여러 사용자가 Office에 액세스할 수 있습니다.

1. [머신별 모드에 OneDrive 설치](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode) 일반적으로 OneDrive는 사용자당 설치되지만 여기서는 머신당 설치해야 합니다.