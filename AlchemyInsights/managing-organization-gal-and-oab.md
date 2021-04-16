---
title: 조직 전체 주소 목록 및 오프라인 주소록 관리
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
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794838"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>조직 전체 주소 목록(GAL) 및 오프라인 주소록 관리(OAB)

전체 주소 목록(GAL)은 조직에서 메일 사용이 가능한 개체(전자 메일을 받을 수 있는 모든 받는 사람 유형)의 목록입니다. 모든 조직에서 GAL은 자동으로 생성됩니다. 조직이나 위치별로 사용자를 구분할 추가 GAL를 만들 수 있지만, 단일 사용자는 한 번에 하나의 GAL만 보고 사용할 수 있습니다.

Windows용 Outlook과 같은 일부 전자 메일 클라이언트는 오프라인 사용을 위해 GAL을 다운로드합니다. 이를 오프라인 주소록(OAB)이라고 합니다. Exchange online에서 OAB는 8시간 마다 한 번만 업데이트되고 그 후 클라이언트는 이를 다운로드하여 로컬 OAB 복사본을 업데이트해야 합니다. 모든 받는 사람에 대한 변경 내용은 먼저 GAL에서 확인되어야 하고 이후에 OAB에서 확인할 수 있도록 합니다.

일반적으로 사용되는 GAL과 OAB 절차는 다음과 같습니다.

- 다양한 이유로 GAL에서 일부 개체를 숨기는 것이 좋습니다. [주소 목록에서 받는 사람 숨기기](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists)를 참조하세요.
- 특정 사용자 그룹에 조직의 GAL에 대한 사용자 지정 보기를 제공해야 하는 경우에는 [Exchange Online에서의 주소록 정책](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies)을 참조하세요.
- [Exchange Online에서 전체 주소 목록 만들기](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list)를 수행하고 GAL 사용 권한을 작업하는 방법에 대한 내용은 [Exchange Online에서의 주소 목록](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists)을 참조하세요. 새 GAL을 만드는 경우 새 OAB를 만드는 것이 좋을 수도 있습니다. [오프라인 주소록 절차](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures)를 참조하세요.
