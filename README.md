# EnvReader
## 使い方
`EnvReader::getParams(string $path);`
を呼び出す。
`require`を忘れずに！

注意！
.envファイル内では以下のように記述すること
```
NAME=AAA
```
[string => string]で配列が作られるため数値を入れたい場合は注意
後=の後にスペースを入れないこと

```
echo '<pre>';
var_dump(DataBaseMethod::getParams());
echo '</pre>';
```
をコメントアウトすることでどのように読み込まれているか確かめることができます。

今後機能追加として、
- イコールの後に空白OKにする。
- 数値をそれぞれの方に変換する。
などをするかもしれない（余裕があれば）
