####################################
パーソナライズの条件
####################################

このトピックでは、Sitecore Experience Platform (XP) と Sitecore Experience Manager (XM) で利用可能なパーソナライゼーション条件をリストアップします。

完全に設定されたSitecore XPのインストールでは、Rule Set Editorのすべてのパーソナライゼーション条件を使用することができ、ヒストリカルパーソナライゼーションとセッション内パーソナライゼーションを実装することができます。

しかし、Sitecore XMのインストールでは、Sitecore XMのインストール方法によって使用できるパーソナライゼーション条件が異なります。

* Sitecore XP トポロジーパッケージ（XP Scaled または XP Single）を使用して Sitecore XP をインストールし、CMS 専用モードで実行するように設定した場合、パーソナライゼーション条件の一部が利用可能で、セッション内パーソナライゼーションを実装することができます。
* Sitecore XM Scaled トポロジーパッケージを使用して Sitecore XM をインストールした場合、パーソナライゼーション条件は利用できず、パーソナライゼーションを実装することはできません。

Commerce Connectをインストールした場合は、Commerce Connect用のパーソナライゼーション条件が追加でインストールされます。

ルールセットエディタでは、パーソナライゼーション条件はカテゴリごとに整理されています。カテゴリは以下の通りです。

* キャンペーン
* チャンネル
* 日付
* デバイス
* フィールド
* IP Geolocation
* アイテム海藻
* アイテム情報
* アイテムバージョン
* マーケティングオートメーション
* セキュリティ
* Sitecore クエリ
* システム
* トラッキング
* 会場
* 訪問
* 訪問者
* xDB

以下の表のルールはすべてXPで使用できます。XMで使用できる条件は、互換性がある(Yes)、またはサポートされていない(No)とマークされています。

* XM-1 Sitecore XMトポロジーパッケージと一緒にインストール
* XM-2 Sitecore XPをCMSオンリーモードで実行するように設定されています。

**************************
定義済みのルール
**************************


+----------------------------+-------+-------+-----+
| 条件                       | XM-1  | XM-2  | XP  |
+----------------------------+-------+-------+-----+
| 定義済みのルールが真の場合 | No    | Yes   | Yes |
+----------------------------+-------+-------+-----+

******************************
キャンペーン
******************************

+----------------------------------------------------------------------------------------------------------------------+-------+--------------------------------------------------+-----+
| 条件                                                                                                                 | XM-1  | XM-2                                             | XP  |
+----------------------------------------------------------------------------------------------------------------------+-------+--------------------------------------------------+-----+
| 現在のインタラクションのキャンペーンのカスタムファセットフィールドが、指定されたカスタムグループに分類されている場合 | No    | Yes - セッション内パーソナライゼーションのみ対応 | Yes |
+----------------------------------------------------------------------------------------------------------------------+-------+--------------------------------------------------+-----+

******************************
チャンネル
******************************

+--------------------------------------------------------------------------------+-------+-------+-----+
| 条件                                                                           | XM-1  | XM-2  | XP  |
+--------------------------------------------------------------------------------+-------+-------+-----+
| 現在のインタラクションが指定されたチャンネル上にある場合                       | No    | Yes   | Yes |
+--------------------------------------------------------------------------------+-------+-------+-----+
| 現在のインタラクションが指定されたチャンネルグループ内のチャンネル上にある場合 | No    | Yes   | Yes |
+--------------------------------------------------------------------------------+-------+-------+-----+
| 現在のインタラクションが、指定されたチャンネルタイプのチャンネル上にある場合   | No    | Yes   | Yes |
+--------------------------------------------------------------------------------+-------+-------+-----+

******************************
日付
******************************

+----------------------------------+-------+-------+-----+
| 条件                             | XM-1  | XM-2  | XP  |
+----------------------------------+-------+-------+-----+
| 日にちが経過した場合             | No    | Yes   | Yes |
+----------------------------------+-------+-------+-----+
| 現在の月の日と数字を比較した場合 | No    | Yes   | Yes |
+----------------------------------+-------+-------+-----+
| 現在の日が曜日の場合             | No    | Yes   | Yes |
+----------------------------------+-------+-------+-----+
| 現在の月が月の場合               | No    | Yes   | Yes |
+----------------------------------+-------+-------+-----+

******************************
デバイス
******************************

+----------------------------------------------------------------------------+-------+-------+-----+
| 条件                                                                       | XM-1  | XM-2  | XP  |
+----------------------------------------------------------------------------+-------+-------+-----+
| デバイスブラウザが特定の値と比較する場所                                   | No    | Yes   | Yes |
+----------------------------------------------------------------------------+-------+-------+-----+
| ブラウザがHTML 5のオーディオをサポートしている場所                         | No    | Yes   | Yes |
+----------------------------------------------------------------------------+-------+-------+-----+
| ブラウザがHTML 5の動画をサポートしている場所                               | No    | Yes   | Yes |
+----------------------------------------------------------------------------+-------+-------+-----+
| ブラウザがJavaScriptをサポートしている場所                                 | No    | Yes   | Yes |
+----------------------------------------------------------------------------+-------+-------+-----+
| デバイスがボットになっている場所                                           | No    | Yes   | Yes |
+----------------------------------------------------------------------------+-------+-------+-----+
| デバイスのハードウェアモデルが特定の値と比較される場合                     | No    | Yes   | Yes |
+----------------------------------------------------------------------------+-------+-------+-----+
| デバイスのプロパティが特定の値と比較される場所                             | No    | Yes   | Yes |
+----------------------------------------------------------------------------+-------+-------+-----+
| デバイスのオペレーティングシステムが特定の値と比較する場合                 | No    | Yes   | Yes |
+----------------------------------------------------------------------------+-------+-------+-----+
| デバイス・オペレーティング・システム・ベンダーが特定の値と比較している場所 | No    | Yes   | Yes |
+----------------------------------------------------------------------------+-------+-------+-----+
| デバイスがタッチスクリーンをサポートしている場合                           | No    | Yes   | Yes |
+----------------------------------------------------------------------------+-------+-------+-----+
| デバイスタイプがリストのいずれかである場合                                 | No    | Yes   | Yes |
+----------------------------------------------------------------------------+-------+-------+-----+
| デバイスベンダーが特定の値と比較しているところ                             | No    | Yes   | Yes |
+----------------------------------------------------------------------------+-------+-------+-----+
| ハードウェア画面の高さと数字の比較                                         | No    | Yes   | Yes |
+----------------------------------------------------------------------------+-------+-------+-----+
| ハードウェアの画面幅と数値の比較                                           | No    | Yes   | Yes |
+----------------------------------------------------------------------------+-------+-------+-----+

******************************
フィールド
******************************

+--------------------------------------------------------------------------+-------+-------+-----+
| 条件                                                                     | XM-1  | XM-2  | XP  |
+--------------------------------------------------------------------------+-------+-------+-----+
| 特定のフィールドが特定の値と比較される場合                               | No    | Yes   | Yes |
+--------------------------------------------------------------------------+-------+-------+-----+
| 特定のフィールドが空の場合                                               | No    | Yes   | Yes |
+--------------------------------------------------------------------------+-------+-------+-----+
| 項目に特定のフィールドタイプと比較するフィールドタイプが含まれている場合 | No    | Yes   | Yes |
+--------------------------------------------------------------------------+-------+-------+-----+

******************************
IP Geolocation
******************************

+----------------------------------------+-------+-------+-----+
| 条件                                   | XM-1  | XM-2  | XP  |
+----------------------------------------+-------+-------+-----+
| 市外局番が特定の値と比較される場所     | No    | Yes   | Yes |
+----------------------------------------+-------+-------+-----+
| 事業名と特定の値を比較する場合         | No    | Yes   | Yes |
+----------------------------------------+-------+-------+-----+
| 特定の都市と比較した場合               | No    | Yes   | Yes |
+----------------------------------------+-------+-------+-----+
| 特定の国と比較しているところ           | No    | Yes   | Yes |
+----------------------------------------+-------+-------+-----+
| DNSアドレスが特定の値と比較される場所  | No    | Yes   | Yes |
+----------------------------------------+-------+-------+-----+
| IP アドレスが特定の値と比較される場合  | No    | Yes   | Yes |
+----------------------------------------+-------+-------+-----+
| ISP名と特定の値を比較する場合          | No    | Yes   | Yes |
+----------------------------------------+-------+-------+-----+
| 緯度が特定の値と比較される場所         | No    | Yes   | Yes |
+----------------------------------------+-------+-------+-----+
| 経度が特定の値と比較される場所         | No    | Yes   | Yes |
+----------------------------------------+-------+-------+-----+
| メトロコードが特定の値と比較される場所 | No    | Yes   | Yes |
+----------------------------------------+-------+-------+-----+
| 郵便番号が特定の値と比較される場合     | No    | Yes   | Yes |
+----------------------------------------+-------+-------+-----+
| 地域が特定の値と比較しているところ     | No    | Yes   | Yes |
+----------------------------------------+-------+-------+-----+

******************************
アイテム階層
******************************

+--------------------------------------------------------+------+------+-----+
| 条件                                                   | XM-1 | XM-2 | XP  |
+--------------------------------------------------------+------+------+-----+
| アイテムが特定の項目またはその祖先のいずれかである場合 | No   | Yes  | Yes |
+--------------------------------------------------------+------+------+-----+
| アイテムが特定の項目またはその子孫のいずれかである場合 | No   | Yes  | Yes |
+--------------------------------------------------------+------+------+-----+
| 項目のレベルと数を比較する場合                         | No   | Yes  | Yes |
+--------------------------------------------------------+------+------+-----+
| アイテムのパスがパスと比較される場所                   | No   | Yes  | Yes |
+--------------------------------------------------------+------+------+-----+
| 親の名前が値と比較される場所                           | No   | Yes  | Yes |
+--------------------------------------------------------+------+------+-----+
| 親テンプレートが特定のテンプレートの場合               | No   | Yes  | Yes |
+--------------------------------------------------------+------+------+-----+

******************************
アイテム情報
******************************

+------------------------------------------------+------+------+-----+
| 条件                                           | XM-1 | XM-2 | XP  |
+------------------------------------------------+------+------+-----+
| アイテムIDが値と比較される場所                 | No   | Yes  | Yes |
+------------------------------------------------+------+------+-----+
| アイテム名と値が比較される場所                 | No   | Yes  | Yes |
+------------------------------------------------+------+------+-----+
| アイテムテンプレートが特定のテンプレートの場合 | No   | Yes  | Yes |
+------------------------------------------------+------+------+-----+

******************************
アイテムバージョン
******************************

+--------------------------------+------+------+-----+
| 条件                           | XM-1 | XM-2 | XP  |
+--------------------------------+------+------+-----+
| 項目の言語が値と比較される場所 | No   | Yes  | Yes |
+--------------------------------+------+------+-----+

******************************
マーケティングオートメーション
******************************

+------------------------------------------------------------------------------------------------------+------+------+-----+
| 条件                                                                                                 | XM-1 | XM-2 | XP  |
+------------------------------------------------------------------------------------------------------+------+------+-----+
| コンタクトが以前に特定のオートメーションキャンペーンに参加していて、開始日と終了日の間に終了した場合 | No   | No   | Yes |
+------------------------------------------------------------------------------------------------------+------+------+-----+
| コンタクトが現在特定のオートメーションキャンペーンに参加している場所                                 | No   | No   | Yes |
+------------------------------------------------------------------------------------------------------+------+------+-----+
| コンタクトが現在、特定のオートメーションキャンペーンの特定の活動に登録され、待機している場合         | No   | No   | Yes |
+------------------------------------------------------------------------------------------------------+------+------+-----+

******************************
セキュリティ
******************************

+----------------------------------------------------------------------+------+------+-----+
| 条件                                                                 | XM-1 | XM-2 | XP  |
+----------------------------------------------------------------------+------+------+-----+
| 現在のユーザが匿名の場合                                             | No   | Yes  | Yes |
+----------------------------------------------------------------------+------+------+-----+
| 現在のユーザードメイン名が値と比較される場所                         | No   | Yes  | Yes |
+----------------------------------------------------------------------+------+------+-----+
| ユーザープロファイルに有効なメールアドレスが含まれている場合         | No   | Yes  | Yes |
+----------------------------------------------------------------------+------+------+-----+
| 現在のユーザー名が値と比較される場所                                 | No   | Yes  | Yes |
+----------------------------------------------------------------------+------+------+-----+
| ユーザープロファイルの特定のフィールドが値と比較される場所           | No   | Yes  | Yes |
+----------------------------------------------------------------------+------+------+-----+
| ユーザープロファイルの特定のフィールドが空でない場合                 | No   | Yes  | Yes |
+----------------------------------------------------------------------+------+------+-----+
| ユーザープロファイルの特定の数値フィールドの値が数値と比較される場所 | No   | Yes  | Yes |
+----------------------------------------------------------------------+------+------+-----+
| 現在のユーザーが特定のロールのメンバーである場合                     | No   | Yes  | Yes |
+----------------------------------------------------------------------+------+------+-----+

******************************
Sitecore クエリ
******************************

+--------------------------------+------+------+-----+
| 条件                           | XM-1 | XM-2 | XP  |
+--------------------------------+------+------+-----+
| 式のクエリの結果が存在する場合 | No   | Yes  | Yes |
+--------------------------------+------+------+-----+

******************************
システム
******************************

+------------------------------------------+------+------+-----+
| 条件                                     | XM-1 | XM-2 | XP  |
+------------------------------------------+------+------+-----+
| 特定のスクリプトの呼び出しが真を返す場合 | No   | Yes  | Yes |
+------------------------------------------+------+------+-----+
| 特定のルールの条件が真の場合             | No   | Yes  | Yes |
+------------------------------------------+------+------+-----+
| コンテンツ検索機能が有効な場合           | No   | Yes  | Yes |
+------------------------------------------+------+------+-----+
| 現在のドメイン名が値と比較される場所     | No   | Yes  | Yes |
+------------------------------------------+------+------+-----+
| アイテムバケット機能が有効な場合         | No   | Yes  | Yes |
+------------------------------------------+------+------+-----+
| 真の場合 (アクションは常に実行されます)  | No   | Yes  | Yes |
+------------------------------------------+------+------+-----+

.. note:: アナリティクスが有効な条件は、Sitecore 8.1で廃止されました。これは、TrackingカテゴリのTrackingが有効な条件に置き換えられ、xDBカテゴリのxDBが有効な条件に置き換えられました。


******************************
トラッキング
******************************

+--------------------+------+------+-----+
| 条件               | XM-1 | XM-2 | XP  |
+--------------------+------+------+-----+
| トラッキングが有効 | No   | Yes  | Yes |
+--------------------+------+------+-----+

******************************
会場
******************************

+------------------------------------------------------------------+------+------+-----+
| 条件                                                             | XM-1 | XM-2 | XP  |
+------------------------------------------------------------------+------+------+-----+
| 現在のインタラクションが指定された会場にある場合                 | No   | Yes  | Yes |
+------------------------------------------------------------------+------+------+-----+
| 現在のインタラクションが指定された会場グループ内の会場にある場合 | No   | Yes  | Yes |
+------------------------------------------------------------------+------+------+-----+
| 現在のインタラクションが指定された会場タイプの会場にある場合     | No   | Yes  | Yes |
+------------------------------------------------------------------+------+------+-----+

******************************
訪問
******************************

.. note:: 訪問者グループの条件は、現在の訪問者と過去の訪問者の両方のデータに基づいています。訪問者の過去の行動のみを考慮した条件については、訪問者グループを参照してください。

+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 条件                                                                                                                                                                           | XM-1 | XM-2 | XP  |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 現在の訪問中に、リスト内のキャンペーンのうち少なくとも1つがトリガーされた場合                                                                                                  | No   | Yes  | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 過去または現在のインタラクション中に特定のキャンペーンがトリガーされた場合、経過日数が数値と比較され、過去のインタラクション数が数値と比較される場合                           | No   | No   | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 過去または現在のインタラクション中に特定のキャンペーンがトリガーされ、経過日数が数値と比較され、過去のインタラクション数が数値と比較され、カスタムデータが数値と比較された場合 | No   | No   | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 過去または現在のインタラクションが特定のチャンネル上にあり、その経過日数が数値と比較される場合、および過去のインタラクション数が数値と比較される場合                           | No   | No   | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 過去または現在のインタラクションが特定のチャンネル上にあり、経過日数が数値と比較され、過去のインタラクション数が数値と比較され、カスタムデータが値と比較される場合             | No   | No   | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| エンゲージメントバリューポイントの数と比較した場合                                                                                                                             | No   | Yes  | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 現在の訪問中に特定の目標が発動した場所                                                                                                                                         | No   | Yes  | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 過去または現在のインタラクション中に特定の目標がトリガーされた場合、経過日数が数値と比較され、過去のインタラクション数が数値と比較された場合                                   | No   | No   | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 過去または現在のインタラクション中に特定のゴールがトリガーされ、経過日数が数値と比較され、過去のインタラクション数が数値と比較され、カスタムデータが数値と比較された場合       | No   | No   | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 現在の訪問が特定のプロファイルの特定のパターンカードと一致する場合                                                                                                             | No   | Yes  | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 特定の結果が過去または現在の相互作用中に登録された場合、経過日数が数値と比較され、過去の相互作用数が数値と比較された場合に、特定の結果が登録される。                           | No   | No   | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 特定のページイベントが過去または現在のインタラクション中にトリガーされた場合、経過日数が数値と比較され、過去のインタラクション数が数値と比較される場合                         | No   | No   | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 特定のページイベントが過去または現在のインタラクション中にトリガーされ、経過日数が数値と比較され、過去のインタラクション数が数値と比較され、カスタムデータが値と比較された場合 | No   | No   | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| ページインデックスと数字を比較した場合                                                                                                                                         | No   | Yes  | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 現在の訪問中に特定のページが訪問された場所                                                                                                                                     | No   | Yes  | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 相互作用プロファイルの特定のプロファイルキーの値が、特定の値と比較される場合                                                                                                   | No   | Yes  | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 検索キーワードが特定の値と比較される場所                                                                                                                                       | No   | Yes  | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| サイト名と値が比較される場所                                                                                                                                                   | No   | Yes  | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| トラフィックタイプが数と比較される場所                                                                                                                                         | No   | Yes  | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 過去または現在の交流が特定の会場で行われている場合で、経過日数が数と比較される場合、過去の交流数が数と比較される場合                                                           | No   | No   | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 過去または現在のインタラクションが特定の会場上にあり、経過日数が数値と比較され、過去のインタラクション数が数値と比較され、カスタムデータが値と比較される場合                   | No   | No   | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| リストのどのページから訪問を開始したか                                                                                                                                         | No   | Yes  | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 開始日と日付を比較する場所                                                                                                                                                     | No   | Yes  | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+
| 参照元が特定の値と比較する場合                                                                                                                                                 | No   | Yes  | Yes |
+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------+------+-----+


******************************
訪問者
******************************

.. note:: 訪問者グループの条件は、コンタクトのプロファイルに蓄積された履歴データに基づいており、複数の訪問からのデータを含めることができます。コンタクトのプロファイルでカバーされるデフォルトの最大期間は30日です。現在の訪問での訪問者の行動を見る条件については、訪問者グループを参照してください。

+-------------------------------------------------------------------------------+------+------+-----+
| 条件                                                                          | XM-1 | XM-2 | XP  |
+-------------------------------------------------------------------------------+------+------+-----+
| コンタクトの現在のエンゲージメントバリューポイントの数と比較した場合          | No   | No   | Yes |
+-------------------------------------------------------------------------------+------+------+-----+
| 現在の連絡先が指定された連絡先リストにある場合                                | No   | No   | Yes |
+-------------------------------------------------------------------------------+------+------+-----+
| 訪問番号と比較した場合                                                        | No   | No   | Yes |
+-------------------------------------------------------------------------------+------+------+-----+
| 訪問者の特定タグが空でない場合                                                | No   | No   | Yes |
+-------------------------------------------------------------------------------+------+------+-----+
| ISP名と特定の値を比較する場合                                                 | No   | No   | Yes |
+-------------------------------------------------------------------------------+------+------+-----+
| 現在の連絡先がリストのプロフィールパターンカードの少なくとも1つと一致する場合 | No   | No   | Yes |
+-------------------------------------------------------------------------------+------+------+-----+
| 接触行動プロファイルの特定のプロファイルキーの値が特定の値と比較される場合    | No   | No   | Yes |
+-------------------------------------------------------------------------------+------+------+-----+
| ユーザープロファイルの特定の数値フィールドの値が数値と比較される場所          | No   | No   | Yes |
+-------------------------------------------------------------------------------+------+------+-----+
| 訪問者の識別が特定の値と比較される場所                                        | No   | No   | Yes |
+-------------------------------------------------------------------------------+------+------+-----+
| 訪問者の特定のタグが値と比較される場所                                        | No   | No   | Yes |
+-------------------------------------------------------------------------------+------+------+-----+

******************************
xDB
******************************

+------------+------+------+-----+
| 条件       | XM-1 | XM-2 | XP  |
+------------+------+------+-----+
| xDB が有効 | No   | Yes  | Yes |
+------------+------+------+-----+

.. tip:: 英語版 https://doc.sitecore.com/users/93/sitecore-experience-platform/en/the-personalization-conditions.html