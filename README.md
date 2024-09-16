# R-Amano/AorUIController README (日本語)
<img src="/source/pack_icon.png" width="200px" />
Minecraft Bedrock Resource & Behavior  
## Athletic of Round UI Controller とは？ - What's AorUC?
マインクラフト統合版アスレチックゲーム「円形アスレチック・リマスター」二章 より構築を考えているカスタムUIシステム。  
おおよそのテンプレートを作成し、npcダイアログ等にコードを記述する事で様々なUI表現を可能にする。  
テンプレ可する事で自身の制作作業効率化に加え、第三者が円形アスレチック・リマスターにオリジナルのストーリーを展開させる事も可能と考えている。  

## 参考資料
JSON UI Documentation  
https://wiki.bedrock.dev/json-ui/json-ui-documentation.html  

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

