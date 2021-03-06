##############################
成果
##############################

成果とは、コンタクトとブランドとの対話から得られるビジネス上の重要な成果のことです。コンタクトが顧客になるまでのプロセスを通じて、コンタクトがきっかけとなったイベントと、そのプロセスでコンバージョンしたゴールを追跡することができます。これにより、接触者がどのようにウェブサイトと対話しているか、また接触者が組織にとってどのような財務的価値を持っているかを知ることができます。

成果の例としては、コンタクトの情報を取得したこと、コンタクトが顧客になったこと、顧客が顧客ロイヤルティプログラムに参加したことなどが挙げられます。

成果があれば、エンゲージメントの価値ではなく、コンタクトが組織にもたらした財務的価値に基づいてコンタクトを定量化することができます。財務的価値は金銭的価値に基づくこともできますが、顧客が組織にもたらす価値という観点から、財務的価値をより広く定義することもできます。

例えば、あるコンタクトが自動車販売店のウェブサイトを訪問し、ニュースレターに登録したとします。そのコンタクトは販売店を訪れ、車を購入し、顧客となります。車を購入してから3年後、その顧客は延長保証プランにサインアップし、購入時の金銭的価値に基づいてブランドへの忠誠心を示します。これは、その顧客が将来、そのディーラーから他の車を購入する可能性があり、組織に高い財務的価値を提供していることを示しています。

この例では、成果を使用して車両販売の財務的価値を追跡し、接触者が訪問者からリード、そしてリードから顧客に至るまでのステップを特定することができます。

**************************************
成果とパーソナライゼーション
**************************************

成果物を使用してパーソナライゼーションルールを作成して実装することで、ターゲットを絞った関連性の高いコンテンツをコンタクトに提供することができます。定義された成果物をチェックするパーソナライゼーションルールを設定することで、特定のコンテンツを表示、非表示、または調整することで、リアルタイムで適切なコンテンツが適切な訪問者に届くようにすることができます。

また、成果タイプをトリガーとして使用するマーケティングオートメーションプランを作成することもできます。マーケティングオートメーションプランは、個々のインタラクションに適したコンテンツ、チャネル、メディアを使用するようにコミュニケーションを適応させることで、コンタクトとの関係性を育むのに役立ちます。

カーディーラーの例では、会社はニュースレターにサインアップした後、コンタクトをオートメーションプランに登録することができる。車を購入することがトリガーとなり、顧客を別のオートメーションプランの状態にすることができます。会社は、Eメール・エクスペリエンス・マネージャーを使用して、その特定の顧客に関連するパーソナライズされたメッセージを定期的に送信することができます。顧客との良好な関係を維持することで、企業は顧客を維持し、ブランドロイヤルティを高め、生涯にわたって顧客を獲得することができます。

**************************************
カスタム成果物の作成
**************************************

マーケティングコントロールパネルでは、マーケッターは成果グループと成果を作成することができます。開発者は、プログラムで成果物を作成して登録することができます。

マーケティングコントロールパネルでは、成果は以下のように構造化されています。

成果グループ - 成果定義アイテムを含むカテゴリ。例えば、「購入」など。

成果 - 特定の成果アイテム。たとえば、「製品購入」は、「購入タイプ」の成果物です。

**************************************
成果の登録
**************************************

成果グループまたは成果定義アイテムを作成した後、成果をトリガーにしたい場合は、開発者が登録する必要があります。成果は自動的には登録されません。カスタムでも定義済みでも、すべての成果はプログラムで登録する必要があります。

成果は、連絡先が Web サイトの特定のページを訪問したときに発生したり、外部システムでトリガーされたりします。成果がトリガーされると、それはコンタクトに添付され、xDB コレクションデータベースに保存されます。

**************************************
定義済みの成果
**************************************

マーケティングコントロールパネルには、3つのデフォルトの成果グループがあります。各成果グループには、いくつかの定義済み成果があります。

* 識別 - コンタクト獲得を識別する
* 購入 - 商品が購入されたことを示します。
* リード管理ファネル - リード管理ファネルを介して進行するコンタクトを識別することができます。リード管理ファネル内には、いくつかの成果物の定義があります。これらは、マーケティングコントロールパネルの「成果」の下にあります。これらは以下の通りです。

+----------------------+-------------------------------------------------------------------------------------------------------------------------------------------------+
| 成果の定義           | 説明                                                                                                                                            |
+----------------------+-------------------------------------------------------------------------------------------------------------------------------------------------+
| マーケティングリード | ホワイトペーパーのダウンロードやウェビナーへの参加など、特定のアクションを行ったが、まだ顧客ではないマーケティング適格リード（MQL）。           |
+----------------------+-------------------------------------------------------------------------------------------------------------------------------------------------+
| セールスリード       | 興味を持っているリードであり、購買決定を行う能力を持っている販売資格のあるリード（SQL）。これらのコンタクトは、通常、営業チームに転送されます。 |
+----------------------+-------------------------------------------------------------------------------------------------------------------------------------------------+
| 販売機会             | 顧客になることを計画している有資格者のリード。                                                                                                  |
+----------------------+-------------------------------------------------------------------------------------------------------------------------------------------------+
| クローズウォン       | 顧客となったクローズドリード。                                                                                                                  |
+----------------------+-------------------------------------------------------------------------------------------------------------------------------------------------+
| クローズロスト       | お客様にならなかったクローズドリード。                                                                                                          |
+----------------------+-------------------------------------------------------------------------------------------------------------------------------------------------+
| クローズキャンセル   | 顧客だったが契約を解除したクローズドリード。                                                                                                    |
+----------------------+-------------------------------------------------------------------------------------------------------------------------------------------------+
| 連絡先取得           | 獲得した新しいコンタクト                                                                                                                        |
+----------------------+-------------------------------------------------------------------------------------------------------------------------------------------------+
| 製品購入             | 連絡先が商品を購入した                                                                                                                          |
+----------------------+-------------------------------------------------------------------------------------------------------------------------------------------------+

.. tip:: 英語版 https://doc.sitecore.com/users/93/sitecore-experience-platform/en/outcomes.html

.. toctree::
    :hidden:
    :maxdepth: 1

    create-an-outcome-group-and-an-outcome
    