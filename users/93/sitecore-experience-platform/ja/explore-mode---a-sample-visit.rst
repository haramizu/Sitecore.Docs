#######################################
エクスプローラーモード - 訪問サンプル
#######################################

エクスペリエンスモードを使用して、実際の訪問者の視点からウェブサイトを訪問したときの体験をシミュレートします。プリセットを選択すると、対応するプリセットで指定された重要なビジネスターゲットグループの1つに合わせて、訪問中にウェブサイトのルック＆フィールが調整されます。訪問をシミュレートするには、2つの方法があります。

* 固定訪問では、訪問者がウェブサイトをナビゲートすると、すべてのプロファイル値が自動的に選択されたプリセットで指定された値にリセットされます。固定訪問では、ウェブサイトの各ページは、訪問者が最初のページとしてそのページに直接アクセスしたか、プロフィールを固定したままにしているかのように表示されます。
  つまり、訪問中にトリガーされた目標、キャンペーン、またはプロフィールの値は自動的にリセットされ、訪問中の値として蓄積されないということです。
* ジャーニー訪問では、訪問者がウェブサイトをナビゲートすると、すべての値が蓄積され、これらの値が訪問者に追従するため、訪問が実際の旅をシミュレートします。
  つまり、訪問中にトリガーされた目標、キャンペーン、またはプロファイルの値は、訪問者に自動的に関連付けられ、訪問中に蓄積されます。

****************
プリセット
****************

プリセットとは、目標、キャンペーン、プロフィールの値、または条件付きレンダリングなどの値が関連付けられたペルソナのことです。SBOSチームは、あなたのウェブサイトで使用するための適切なプリセットを開発するお手伝いをします。

この例では、プリセットを使用しています。

* セシール - ファーストクラスを利用し、高水準のビジネス宿泊施設を期待する会社のCEO。

このシナリオでは、セシルがジェットストリームのウェブサイトの様々なページを訪れたときの体験をシミュレートしています。彼女がウェブサイトをナビゲートしながら、目標を達成したり、行動を変えたり、サイトの異なるページを訪れたりすることで、ウェブサイトが彼女の動きに合わせて変化していく様子を見ることができます。

このシナリオでは、固定訪問とジャーニー訪問の違いについても説明しています。


プリセットの選択
=================

ウェブサイトへの訪問をシミュレートする前に、適切なプリセットを選択する必要があります。

エクスプローラーモードのプリセットを選択するには、以下の手順に従います。

1. エクスペリエンスエディタで、モードグループのExploreをクリックします。
2. [設定]パネルで[エクスペリエンス]セクションを展開し、関連するプリセット（例：Cecile）を選択します。
3. パネルの上部で、該当する探索モード（固定またはジャーニー）を選択します。
4. 適用をクリックします。

ホームページ
===============

ジェットストリームのウェブサイトでは、デフォルトのホームページにヴェネツィアの情報が表示されています。

.. image:: images/15eafd358578e5.png
   :align: center
   :width: 400px
   :alt: ホームページ

ビューア パネルの [ページ構成] セクションで、ヒーロー カルーセル スポットでは、パーソナライズ ルールが発動されていないことがわかります。

.. image:: images/15eafd3585eed8.png
   :align: center
   :alt: ホームページ

セシールがウェブサイトを訪問した場合、ホームページにはパリの情報が表示されますが、これは主にセシールのパーソナライゼーションルールで指定されているためです。

.. image:: images/15eafd3586530d.png
   :align: center
   :width: 400px
   :alt: ホームページ

ビューアパネルのページ設定セクションで、固定とジャーニーの両方の訪問の場合、ヒーローカルーセルスポットでは、「Mostly Cecile」パーソナライゼーションルールが適用され、太字で緑色のアイコンが表示されていることがわかります。これは、セシールのプリセット値がこのパーソナライゼーションルール（Mostly Cecile）に指定された値と密接に一致しているためです。

.. image:: images/15eafd3586c2ec.png
   :align: center
   :alt: ホームページ

目的地ページ
==============

セシルは可能性のある目的地に興味を持ち、目的地のページに移動します。

.. image:: images/15eafd35872730.png
   :align: center
   :width: 400px
   :alt: 目的地ページ

彼女はカリブ海の目的地をクリックします。

カリブ海は家族連れに人気のある休暇先であるため、イアンのプリセットのより家族向けのプロフィールにマッチしています。イアンは、オールインクルーシブで、家族で楽しめるアクティビティが充実していて、信頼できる託児施設がある休暇先を探している家族派の男性です。

.. image:: images/15eafd35879996.png
   :align: center
   :width: 400px
   :alt: 目的地ページ

固定訪問では、セシルがカリブのページを訪問すると、セシルのイアンペルソナのプロフィールキーに20ポイントが加算されます。これは、イアンのペルソナが最も支配的になっているためです。

.. image:: images/15eafd3588029a.png
   :align: center
   :alt: 目的地ページ

この値は、彼女がこのページを閲覧したときにのみ表示されます - 彼女がページを離れると、セシルのプリセットの値は0にリセットされます。

ジャーニー訪問では、セシルがカリブ海のページを訪問すると、イアンのペルソナプロフィールキーに合わせてパーソナライズされ、値のポイントが保持されます。

ホームページに戻る
=====================

セシールはホームページに戻ります。

固定訪問では、すべての値が自動的にリセットされ、要求された各ページで選択されたプリセットと一致するため、固定訪問では、彼女はまだパリについてのフロントページを見ています。イアンのプロフィールに追加された20ポイントのプロフィール値はゼロにリセットされ、代わりにセシールのプリセットで指定されたプロフィール値が追加されます。

.. image:: images/15eafd35886ae8.png
   :align: center
   :width: 400px
   :alt: ホームページに戻る

.. image:: images/15eafd3588d33e.png
   :align: center
   :alt: ホームページに戻る

.. image:: images/15eafd35894180.png
   :align: center
   :width: 400px
   :alt: ホームページに戻る

ジャーニーの訪問では、セシルが家族旅行先を選択したため、ホームページがイアンのプロフィール用にパーソナライズされるようになりました。

セシールのプロフィールが10ポイントしかないのに対し、イアンのプロフィールは20ポイントを獲得しており、今回の訪問ではイアンのプロフィールが最も優位に立っています。このため、ホームページには、一般的な出張先ではなく、家族旅行の目的地に関する情報が表示されます。

.. image:: images/15eafd3589a630.png
   :align: center
   :width: 400px
   :alt: ホームページに戻る

.. image:: images/15eafd358a1672.png
   :align: center
   :alt: ホームページに戻る

.. image:: images/15eafd358a7b58.png
   :align: center
   :alt: ホームページに戻る

ヒーローカルーセルでは、適用されるパーソナライゼーションルールとしてMostly IanがMostly Cecileに置き換わっています。

プロファイルの変更
----------------------

値やプロファイル特性を変更したい場合は、[設定] パネルで直接変更を行うことができます。適用] をクリックすると、現在の訪問の値が更新されます。

たとえば、イアンプロファイルキーの値をゼロまたは50に変更することができます。また、目標やイベントを選択して、目標やイベントがトリガーされた後のサイトの挙動を確認することもできます。

.. note::

  [適用] をクリックしても、実際にはプリセットに定義された値に変更は保存されません。恒久的な変更は、コンテンツ エディタでのみ可能です。
  設定パネルで［リセット］をクリックすると、Exploreモードで使用されるプロファイル値やその他のxMarketingの値をプリセットの初期設定に戻すことができます。

************************************
ニュースレターのサインアップページ
************************************

セシルはジェットストリームのニュースレターに登録することにしました。彼女がフォームを送信すると、ジェットストリームニュースレターのサインアップフォームのゴールがトリガーされ、彼女の訪問に5つのエンゲージメントバリューポイントが追加されます。

.. image:: images/15ed64a1de7f58.png
   :align: center
   :width: 400px
   :alt: ニュースレターのサインアップページ

.. image:: images/15ed64a1dec595.png
   :align: center
   :width: 400px
   :alt: ニュースレターのサインアップページ

固定訪問では、送信フォームボタンに適用されるゴールはトリガーされません。

.. image:: images/15ed64a1df0731.png
   :align: center
   :width: 400px
   :alt: ニュースレターのサインアップページ

ジャーニー訪問では、オンサイト行動のセクションで、目標が登録され、セシルが5つのエンゲージメントバリューポイントを獲得していることがわかります。セシールのプリセットには、彼女がすでに達成しているいくつかの目標が設定されており、さらに70のエンゲージメントバリューポイントが付与されています。彼女がメルマガに登録した後は、合計75のエンゲージメントバリューポイントを獲得しています。

.. image:: images/15ed64a1e009d1.png
   :align: center
   :alt: ニュースレターのサインアップページ

*********
検索
*********

セシールは、コペンハーゲンからカリブ海のプンタカナへのフライトを検索することにしました。

固定訪問では、セシールが検索結果ページにいるとき、他のトリガーされたゴールは表示されません。セシールの検索では結果は出ませんが、彼女の検索ではフライト検索のゴールがトリガーされます。

.. image:: images/15ed64a1e04d00.png
   :align: center
   :width: 400px
   :alt: 検索

.. image:: images/15ed64a1e093ef.png
   :align: center
   :alt: 検索

ジャーニーの訪問では、フライトサーチのゴールは、彼女のプロフィールにさらに10のエンゲージメントバリューポイントを追加します。

.. image:: images/15ed64a1e0df8d.png
   :align: center
   :width: 400px
   :alt: 検索

.. image:: images/15ed64a1e1276a.png
   :align: center
   :alt: 検索

結果は見つかりませんでしたので、セシルは別のフライトを探すことにしました。この検索を行うと、さらに10のエンゲージメントポイントが加算されます。

.. image:: images/15ed64a1e16fac.png
   :align: center
   :width: 400px
   :alt: 検索


******************
航空券の選択ページ
******************

今回、彼女の検索では、いくつかのフライトが出てきます。彼女は適切なフライトを選択して予約します。このページでは、彼女は再びフライト検索のゴールを起動しました。

.. image:: images/15ed64a1e1b9b8.png
   :align: center
   :width: 400px
   :alt: 航空券の選択ページ


固定訪問では、他のトリガーとなるゴールは表示されません。

ジャーニー訪問では、フライトを予約することで70点のエンゲージメントバリューポイントが追加され、セシルのプロフィールは合計165点となります。

*********************
サンキューページ
*********************

.. image:: images/15ed64a1e1fdcb.png
   :align: center
   :width: 400px
   :alt: サンキューページ

サンキューページでは、セシールは予約ゴールをトリガーにしました。

固定訪問では、現在のページでトリガーされたゴールのみが表示されるため、予約ゴールが表示され、フライト検索ゴールは表示されなくなります。

.. image:: images/15ed64a1e23ffd.png
   :align: center
   :alt: サンキューページ

しかし、旅の訪問では、彼女の旅のビューアパネルには、この訪問中にセシルも3つの追加目標を達成していることが表示されています。

.. image:: images/15ed64a1e28372.png
   :align: center
   :alt: サンキューページ

.. tip:: 英語版 https://doc.sitecore.com/users/93/sitecore-experience-platform/en/explore-mode---a-sample-visit.html


