markdownの書き方チートシート


# 見出し
### 記述例
1個から６個シャープで見出しを記述する。

```
# 見出し内容
```
※スペースを開ける

### 表示例

# 見出し１
## 見出し２
### 見出し３
#### 見出し４
##### 見出し５
###### 見出し６

# 箇条書きリスト
### 記述例
```
- リスト1
  - ネスト リスト1_1
    - ネスト リスト1_1_1
    - ネスト リスト1_1_2
  - ネスト リスト1_2
- リスト2
- リスト3
```
※「*」「+」でも可
### 表示例
- リスト1
  - ネスト リスト1_1
    - ネスト リスト1_1_1
    - ネスト リスト1_1_2
  - ネスト リスト1_2
- リスト2
- リスト3

# 番号付きのリスト
### 記述例
```
1. 番号付きリスト1
    1. 番号付きリスト1_1
    1. 番号付きリスト1_2
1. 番号付きリスト2
1. 番号付きリスト3
```

### 表示例
1. 番号付きリスト1
    1. 番号付きリスト1_1
    1. 番号付きリスト1_2
1. 番号付きリスト2
1. 番号付きリスト3

# 引用
### 記述例
```
> お世話になります。 xxxです。
>　
> ご連絡いただいた、バグの件ですが、仕様となります。
```

### 表示例
> お世話になります。 xxxです。
>
> ご連絡いただいた、バグの件ですが、仕様となります。

※改行をしたい場合の「>」の次にはスペースを入れない。

下は改行を入れた場合の見え方
> お世話になります。 xxxです。
>　
> ご連絡いただいた、バグの件ですが、仕様となります。

１行になっている。
# 二重引用
### 記述例
```
> お世話になります。xxxです。
>
>ご連絡いただいた、バグの件んですが、仕様となります。
>> お世話になっております。yyyです。
>>
>> あの新機能バグがありますね。
```

### 表示例
> お世話になります。xxxです。
>
>ご連絡いただいた、バグの件んですが、仕様となります。
>> お世話になっております。yyyです。
>>
>> あの新機能バグがありますね。

# pre記法(スペース4 or タブ)
### 記述例
```
    # Tab
    class Hoge
        def hoge
            print 'hoge'
        end
    end

---

    # Space
    class Hoge
        def hoge
            print 'hoge'
        end
    end
```
### 表示例
    # Tab
    class Hoge
        def hoge
            print 'hoge'
        end
    end

---

    # Space
    class Hoge
        def hoge
            print 'hoge'
        end
    end

# code記法
### 記述例
```
インストールコマンドは `gem install hoge` です
```
### 表示例
インストールコマンドは `gem install hoge` です

# 強調：<em>
### 記述例
```
normal *italic* normal

normal _italic_ normal
```
### 表示例
normal *italic* normal

normal _italic_ normal

# 強調：<strong>
### 記述例
```
normal **bold** normal

normal __bold__ normal
```
### 表示例
normal **bold** normal

normal __bold__ normal

# 取り消し線
### 記述例
```
~~削除しました。~~
```
### 表示例
~~削除しました。~~

# 水平線
### 記述例
```
***

---

- - - 

* * *
```
※連続するハイフンなどの間にスペースが入ってもよい
### 表示例
***

---

- - - 

* * *

# リンク
### 記述例
```
[google](https://www.google.co.jp/)
```
### 表示例
[google](https://www.google.co.jp/)

# 定義参照リンク
### 記述例
```
[こっちからgoogle][google]
その他の文章
[こっちからもgoogle][google]
```
### 表示例

[こっちからgoogle][google]

その他の文章

[こっちからもgoogle][google]

# 折り畳み
### 記述例
```
<details><summary>タイトル</summary><div>
\```
内容
\```
</div></details>
```

### 表示例
<details><summary>タイトル</summary><div>
```
内容
```
</div></details>

# CheckBox型
### 記述例
```
```
### 表示例
- [ ] タスク１
- [X] タスク２

# テーブル
### 記述例
```
|left align|right align|center aling|
|:--|--:|:--:|
|This|This|This|
|column|column|column|
|will|will|will|
|be|be|be|
|left|right|center|
|aligned|aligned|aligned|
```
### 表示例
|left align|right align|center aling|
|:--|--:|:--:|
|This|This|This|
|column|column|column|
|will|will|will|
|be|be|be|
|left|right|center|
|aligned|aligned|aligned|

# 数式の挿入
### 記述例
```
\```math
\left( \sum_{k=1}^n a_k b_k \right)^{!!2} \leq
\left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)
\```
```
### 表示例
```math
\left( \sum_{k=1}^n a_k b_k \right)^{!!2} \leq
\left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)
```
※他にも「yaml」「json」などのファイル形式も使える