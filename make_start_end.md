# ゲーム開始・終了の追加(How to add game start and end)

## 前提(Premise)
このドキュメントでは前提条件として、monsters_v1がすでにできていることとします。

もしmonsters_v1を作成していない場合は先に、[こちらからmonsters_v1](https://github.com/jincho-ntttx/monsters_v1)を作成してから実施してください。

This document assumes monsters_v1 has been completed.

 If you don't make monsters_v1,please make [monsters_v1](https://github.com/jincho-ntttx/monsters_v1).

## 完成イメージ(Completed image)
- ステージのスプライト

    Compleate Stage sprite.

![stage_comp](figure/stage_comp.png)

- messageのスプライト

    Compleate Message sprite.

![message_comp](figure/message_comp.png)

- Centaurのスプライト

    Compleate Centaur sprite.

![centaur_comp](figure/centaur_comp.png)

# プログラムの作り方(How to develop a program)
## ステージの変更(How to change Stage)
- 変数[damage]を追加する。([変数を作る]→[damage]変数を作成。)

    Add new variable.("変数を作る" → create variable named "damage" )

![stage_1](figure/stage_1.png)

![stage_2](figure/stage_2.png)

- [ずっと]のブロックを[(　)まで繰り返す]に置き換える

    Replace [ずっと] with [(　)まで繰り返す]

![stage_3](figure/stage_3.png)

- ステージのスプライトで以下の図の通り、カテゴリごとのブロックをドラック&ドロップし、ブロック同士をつなげる。

    In Stage sprite. As shown in the figure below, drag and drop blocks for each category to connect the blocks.

![stage_4](figure/stage_4.png)

- メッセージ1の右側にある▼ボタンを押し、[新しいメッセージ]を選択。

    新しいメッセージとして[game_start]を作成する。

    Press the ▼ button on the right side of "メッセージ1" to select the "新しいメッセージ".

    Make "game_start" as new message.

![stage_5](figure/stage_5.png)

![stage_6](figure/stage_6.png)

- [[score]を(0)にする]、[[damage]を(0)にする]が作成されている事を確認する。

    Confirm maked "[score]を(0)にする" and "[damage]を(0)にする".

![stage_7](figure/stage_7.png)

- ブロックの数字をダブルクリックし、3に変更する。

    Double-clicking on a number and change the number to 3.

![stage_8](figure/stage_8.png)

- メッセージ1の右側にある▼ボタンを押し、[新しいメッセージ]を選択。

    新しいメッセージとして[game_end]を作成する。

    Press the ▼ button on the right side of "メッセージ1" to select the "新しいメッセージ".

    Make "game_end" as new message.

![stage_9](figure/stage_9.png)

![stage_10](figure/stage_10.png)

## messageのスプライトの作成(How to make message sprite)
- スプライトを新規に追加する。(スプライト追加ボタン[描く]→game start時に出したいメッセージを描く)

    Add new sprite. Draw game start message.

![message_1](figure/message_1.png)

![message_2](figure/message_2.png)

![message_3](figure/message_3.png)

- コスチューム名を[game start]に変更する。

    Change the costume name to "game start".

![message_4](figure/message_4.png)

- コスチュームを追加する。(コスチュームの追加ボタン[描く]→game overの時に出したいメッセージを描く)

    Add new costume. Draw game over message.

![message_5](figure/message_5.png)

![message_6](figure/message_6.png)

![message_7](figure/message_7.png)

- コスチューム名を[game over]に変更する。

    Change the costume name to "game over".

![message_8](figure/message_8.png)

- スプライト名を[message]変更する。

    Change the sprite name to "message".

![message_9](figure/message_9.png)

- コードのタブに移動する。

    Go to tab named "コード".

![message_10](figure/message_10.png)

- messageのスプライトで以下の図の通り、カテゴリごとのブロックをドラック&ドロップし、ブロック同士をつなげる。

    In message sprite. As shown in the figure below, drag and drop blocks for each category to connect the blocks.

![message_11](figure/message_11.png)

![message_12](figure/message_12.png)

### game_startブロックの作成(How to make game_start block)
- game_startのブロックは最後に[隠す]ブロックのある方で作成する。

    The game_start block is created with the block has "隠す" at last.

![message_13](figure/message_13.png)

- game_endの右側にある▼ボタンを押し、[game_start]を選択する。

    Press the ▼ button on the right side of "game_end" to select the "game_start".

![message_14](figure/message_14.png)

- game_startになっている事を確認する。なっていなかった場合は▼ボタンを押し、[game_start]を選択する。

    Confirm "game start". If the block doesn't become "game start", press the ▼ button to select the "game start".

![message_15](figure/message_15.png)

- ブロックの数字をダブルクリックし、5に変更する。

    Double-clicking on a number and change the number to 5.

![message_16](figure/message_16.png)

- ブロックの数字をダブルクリックし、0.1に変更する。

    Double-clicking on a number and change the number to 0.1.

![message_17](figure/message_17.png)

- ブロックの数字が10になっている事を確認する。なっていなかった場合はブロックの数字をダブルクリックし、10に変更する。

    Confirm the number become 10.If the number doesn't become 10, double-clicking on a number and change the number to 10.

![message_18](figure/message_18.png)

### game_endブロックの作成(How to make game_end block)
- game_endのブロックは最後に[隠す]ブロックがない方で作成する。

    The game_end block is created with the block doesn't have "隠す" at last.

![message_19](figure/message_19.png)

- game_overになっている事を確認する。なっていなかった場合は▼ボタンを押し[game_over]を選択する。

    Confirm "game_over". If the block doesn't become "game_over", press the ▼ button to select the "game_over".

![message_20](figure/message_20.png)

- game_startの右側にある▼ボタンを押し、[game over]を選択する。

    Press the ▼ button on the right side of "game_start" to select the "game over".

![message_21](figure/message_21.png)

- ブロックの数字をダブルクリックし、5に変更する。

    Double-clicking on a number and change the number to 5.

![message_22](figure/message_22.png)

- ブロックの数字をダブルクリックし、0.1に変更する。

    Double-clicking on a number and change the number to 0.1.

![message_23](figure/message_23.png)

- ブロックの数字が10になっている事を確認する。なっていなかった場合はブロックの数字をダブルクリックし、10に変更する。

    Confirm the number become 10.If the number doesn't become 10, double-clicking on a number and change the number to 10.

![message_24](figure/message_24.png)

- 左上の画面で作成したメッセージの位置をドラック&ドロップで調整する。

    The message ajust by dragging and dropping at top left screen.

![message_25](figure/message_25.png)

## Centaurのスプライトの作成(How to change Centaur sprite)
- [このクローンを削除する]の直前に[(damage)を(1)ずつ変える]を追加する。  
Centaurが画面の端までいくとダメージを受けます。

    Add "(damage)を(1)ずつ変える" just before "このクローンを削除する".

![centaur_1](figure/centaur_1.png)


- これでゲーム開始・終了の追加は完成です。

    Game start&end program is complete.
