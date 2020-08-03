---
title: 將您的合作夥伴帳戶與另一個夥伴帳戶合併
description: 在合作夥伴中心使用中的 Microsoft 合作夥伴的公司可以合併他們的帳戶。
ms.topic: article
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: 6c2ac5560b77528766a4d0aa068f231e0aa0bc99
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/30/2020
ms.locfileid: "87444954"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a>將您的合作夥伴帳戶與另一個夥伴帳戶合併

**相關角色**

- 帳戶管理員

有兩個或更多公司使用中的 Microsoft 合作夥伴，並在合作夥伴中心擁有帳戶，可以選擇合併他們的帳戶。

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a>當兩個合作夥伴選擇合併其合作夥伴中心帳戶時，會發生什麼事

- 起始合併的夥伴組織將會是合作夥伴通用帳戶（PGA）。

- 受邀組織的 PGA 會成為起始公司的位置。

- 合併帳戶的所有位置都會變成 PGA 底下的位置。

- 帳戶合併完成後，您會在 PGA 設定檔中看到這兩個帳戶的詳細資料，例如位置和使用者。 您無法還原此進程。

- 在此合併期間，會保留所有位置的 MPN 識別碼。

- 使用者的角色會一併停用。 例如，如果使用者已是特定位置的獎勵系統管理員，他們在合併之後仍然會有該角色，而且能夠看到他們在合併之前看到的獎勵。

- Azure AD 租使用者和 CSP 帳戶不會合並，且不會有任何影響。

- 已發行的供應專案和共同銷售與這兩個公司相關聯的管線資料都會保留

### <a name="view-of-merged-accounts"></a>合併帳戶的觀點

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="帳戶合併":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a>如果您已受邀將合作夥伴中心帳戶與另一個合作夥伴中心帳戶合併，該怎麼辦

如果您決定接受合併帳戶的邀請：·您的 MPN 識別碼和位置將會合並至邀請您的合作夥伴帳戶的 PGA。

- 您的使用者將會帶入已合併的帳戶，並將其角色原封不動。

- 在合併之後，這兩家公司都將保留現有的權益和專長，直到續約為止。 在續訂時，系統會將帳戶視為一家公司，而標準更新規則將會生效。

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a>瞭解當合作夥伴選擇合併帳戶時，對程式和權益的影響

- 所有現有的職稱（金級/銀級）、購買（例如 Microsoft 行動套件）和相關權益都會在匯總期間保留。 如果這兩家公司都具有相同的專長認證，但其中一個是金級，而另一個銀級，則會獎勵具有最高專長的專長認證，而合作夥伴在下一次更新之前，會有一組銀級權益和一組黃金優勢。 

- Microsoft 行動套件的最新週年日會在合併之後保留。 例如，如果公司1的週年日是2020年6月的行動套件更新，而公司2行動套件續訂的週年日是2020年10月，Microsoft 將使用10月2020日作為合併公司的新週年日。

- 在合併帳戶和下一次更新之前，每個帳戶都將保留其行動套件和/或專長認證權益。 續訂時，適用標準行動套件和專長認證更新規則。

- 續約時，會為合作夥伴公司的合作夥伴通用帳戶實行專長認證和行動套件所包含的權益：

  - Microsoft 行動套件：合作夥伴公司將能夠購買每個合作夥伴通用帳戶一個行動套件。

  - 專長認證：合作夥伴公司會收到一份核心權益的套件，其與最高的實現相關，再加上合作夥伴適用于每個合作夥伴通用帳戶的專長認證權益。

- 擁有權益均受[Microsoft 合作夥伴網路權益使用指南](https://aka.ms/partner-benefits-use-guide)的影響。 例如：啟用的 O365 E3 權杖在啟用後的12（12）個月內可運作。 在租使用者上啟用權杖的授權之後，這些授權可能不會移至另一個租使用者。

- 這兩家公司的 MCP 識別碼關聯將會保留，並與 PGA MPN 識別碼相關聯。

- 上市和技術優勢是以專長認證核心權益的形式提供。 合併後，建議您檢查銀行和稅務資訊，以確保正確性。

- 如果您的公司是在 Azure 專家的 MSP 計畫中，則會保留權益直到續訂為止。

- 如果您的公司已獲得先進的特製化，則會保留在這兩個帳戶之間。

- 所有軟體保證的券都會保留在這兩個帳戶中。 

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a>邀請公司合併其合作夥伴中心帳戶與您的合作夥伴中心帳戶

>[!Note]
>若要執行合併帳戶，您必須是公司的**帳戶管理員**。

1. 從您的合作夥伴中心儀表板選取 [**設定**]。 

2. 選取 [**帳戶合併**]。

3. 新增位於您想要邀請之帳戶的**夥伴設定檔**中的 MPN 識別碼，以與您合併。 您必須使用其合作夥伴全域 MPN 識別碼。 您不能使用位置 MPN 識別碼。

4. 當您選取 [**合併**] 時，會將邀請傳送給夥伴公司。 當他們接受您的要求時，您可以在合作夥伴中心內起始帳戶合併。 如果公司拒絕合併帳戶的要求，他們可以解釋為什麼他們會拒絕要求。 您可以在 [**合併歷程記錄**] 下，取得所有帳戶合併的清單。

## <a name="next-steps"></a>後續步驟

- [指派使用者角色和權限](permissions-overview.md)

- [確認您的合作夥伴設定檔資訊](update-your-partner-profile.md)

- [新增 Azure 合作夥伴共用服務，讓合作夥伴可以購買 Azure 訂用帳戶供自己使用](shared-services.md)
