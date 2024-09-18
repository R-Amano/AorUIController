# R-Amano/AorUIController README (日本語)
<img src="/source/pack_icon.png" width="200px" />  
Minecraft Bedrock Resource & Behavior  

## はじめに
　AorUIControllerはNPCダイアログにRPG風のUIを作成し、それをカスタムできるシステムです。NPCダイアログのテキストエディタに直接コードを記述する事で、簡単に様々なUIの表現を可能にしたいと考えている。テンプレ可する事で自身の作業効率化に加え、第三者がAorUCが有効な配布ワールドにオリジナルストーリーを展開させる事も可能となる。  
　なお、JSON JIは将来 [OreUI](https://github.com/Mojang/ore-ui) に置き換えられる可能性があるため、使用できなくなる点に注意して下さい。また、一部のコードは既存のコード、例えばボタンやダイアログなどはテンプレートに依存している為、ゲームのアップデートで変更が生じた場合は使用できなくなる可能性にも留意して下さい。

## 参考文献・資料
JSON UI Documentation  
https://wiki.bedrock.dev/json-ui/json-ui-documentation.html  
NPC Dialogs  
https://wiki.bedrock.dev/entities/npc-dialogs.html  

## バージョン - Version
0.0.1 (bata)  

## ライセンス - LICENCE
MIT License.  
[LICENSE](LICENSE)  

## 仕様
### sourceフォルダ
sourceフォルダは基礎となるAorUCのソースコードです。  
ソースコードはゲーム「円形アスレチック・リマスター」用に作られているので、ご自身のゲームに組み込む際は調整が必要です。  

### sampleフォルダ
sampleフォルダは、AorUCの適用を前提とすることで使用できるアセットです。  
サンプルはいくつでも複製、導入することができ、ほとんどの場合はこちらを複製、改変して使用することになります。  

## テストする
まずはsourceフォルダをリソースパック化し、テストワールドに適用させます。  
次にsampleフォルダをアドオンパックにし、同じワールドへ適用させます。  
コマンドラインを開き、npcを召喚します。
```
/summon npc
```
その後、ゲームモードをサバイバルかアドベンチャーモードへ切り替えます。
```
/gamemode 0
```
npcの近くでサンプルのダイアログを開きます。
```
/dialogue open @e[type=npc,c=1] @s ep01
```
ダイアログの「Next」ボタンで次のダイアログへ進められ、AorUCの動作を確認できます。

