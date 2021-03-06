###################################
アイテムのクローンとアンクローン
###################################

クローンとは、元のアイテムの単なるコピーではなく、元のアイテムからフィールドの値を継承したアイテムのことです。元のアイテムのフィールドを更新すると、クローンの対応するフィールドも更新されます。

Sitecore では、アイテムのクローンや、アイテムのブランチ全体のクローンを作成することができます。ブランチとは、親アイテムとそのすべての子孫のことです。

***************************
アイテムをクローンする
***************************

アイテムのクローンを作成するには

1. コンテンツ ツリーで、クローンを作成するアイテムを選択します。
2. [設定] タブの [クローン] グループで [クローン] をクリックします。

.. image:: images/15eafd356b50c2.png
   :align: center
   :width: 400px
   :alt: アイテムをクローンする

3. [クローン アイテム］ダイアログ ボックスで、クローンを保存する場所を選択します。参照] タブでコンテンツ ツリー内の場所に移動するか、[検索] タブで場所を検索することができます。

.. image:: images/15eafd356ba968.png
   :align: center
   :width: 400px
   :alt: アイテムをクローンする

4. クローンをクリックします。

コンテンツ エディタでクローンアイテムを選択すると、フィールドのタイトルに [元の値] テキストが追加されていることに気づきます。これは、これらの値が元のアイテムの対応する値と一致し、元のアイテムのフィールドを編集した場合に更新されることを意味します。

.. image:: images/15eafd356c1679.png
   :align: center
   :width: 400px
   :alt: アイテムをクローンする

.. important:: ワークフロー内のアイテムをクローンすると、ワークフローとワークフロー状態のプロパティがクローンアイテムにコピーされます。ワークフローフィールドのコピー後は、クローンのワークフロープロパティと元のアイテムのワークフロープロパティは接続されません。元のアイテムのワークフロー状態を変更しても、クローンのワークフロー状態は変わりません。

*************************
アイテムのアンクローン
*************************

元のアイテムとクローンの間の接続を不要にしたい場合は、クローンアイテムのクローンを解除することができます。

クローンアイテムのクローンを解除するには

1. クローンを解除するクローンを選択します。
2. [設定] タブの [クローン] グループで、[クローンの解除] をクリックします。

.. image:: images/15eafd356c7d5e.png
   :align: center
   :width: 400px
   :alt: アイテムをクローンする

クローンアイテムのフィールド値は変更されません。クローンと元のアイテムとの接続が解除され、クローンは通常のコンテンツアイテムになります。



.. tip:: 英語版 https://doc.sitecore.com/users/93/sitecore-experience-platform/en/clone-and-unclone-an-item.html
