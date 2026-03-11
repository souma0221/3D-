# 3D-
命名規則
privateで宣言する変数は小文字から始まり、単語の間は大文字で区切る
hogeFuga

メソッド名、クラス名、構造体名、列挙型名はアクセス修飾子に関わらず大文字から始まり、単語の間も大文字で区切る
HogeMethod、HogeClass、HogeStruct、HogeEnum

定数は全て大文字で単語の区切りにアンダースコア'＿'を使う
HOGE_FUGA

bool型を返す変数やメソッドにはis/has/canを使用すること(以下「bool命名規則」)
isGround、hasItem、canSwim

bool型の命名時、否定する単語を入れない
×isNotDead

abstractクラスは最後にBaseをつけること
AbstractBase

Unityに存在する命名は極力避ける
rigidbody→playerRigidbody

クラス名と同じ名前のpublic変数は命名しない
×public Hoge Hoge { get; }

条件式規則
早期リターンを徹底する
条件式が長くなる場合は改行するのではなく新しい変数を宣言する
// 例
if(abc == ABC && def <= DEF ghi != GHI)
{

}

bool isAbc = abc == ABC;
bool isDef = def <= DEF;
bool isGhi = ghi != GHI;
if(isAbc && isDef
isGhi)
{

}

コメント規則
メソッドの上にはsummaryをつける。
複雑な処理を行う場合、コメントを追記する。
