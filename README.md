# 再利用可能ファイルまとめ
また使いそうだなという部品を独立したモジュールにしておく。
また、利用したモジュールはどんどん改善してまたここに上げて下さい。

- js
- scss
- html
- phpなど

# 決まり事
## scss
- 全てclass指定（idは使わない）
- ファイル名にprefixとして　_module_　をつける
- 変数にprefixとして　M_ をつける
- BEM思考
    1. Block(くくり)、element(Block以下にある全ての要素)、modify(elementの派生 ex)色を変える。消える。動く。など)の３つに分けて考える。
    2. B_E-Mと２種類のバーをつかって表現する。アンダーバーの後はelement。ハイフンの後はmodify。(バーは２つ重ねない)
    3. elementは2階層以下でもあいだの階層は書かない。ex)Block_elementA_elementB => Block_elementB）
    4. jsで後から付けるmodifyの場合、prefixとして is を付ける。ex) -isMoving, -isHidden

# コメントの書き方（コピペして使って下さい）

```css
/*
    [モジュラー名]　ver.x.x (もっといいバージョンの付け方とかあればそれで)
     部品
        xxxxxxxx
         - xxxxx (関数とかcssならクラス名とか)
         - xxxxx (関数とかcssならクラス名とか)
        xxxxxxxx
         - xxxxx (関数とかcssならクラス名とか)
         - xxxxx (関数とかcssならクラス名とか)
    使い方
        1.
        2.
        3.
    バグ
        xxx
        xxx
*/

/* 変数 */
var xxxxx = ; // デフォルト値
var xxxxx = ; // デフォルト値
var xxxxx = ; // デフォルト値

/* モジュール本体 */
モジュール共通部分

/* 自由記述（自分のプロジェクトに合わせて記述。） */

```
