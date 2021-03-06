# the-craft-of-selfteaching

> One has no future if one couldn't teach themself<a href='#fn1' name='fn1b'><sup>[1]</sup></a>.

# 自學是門手藝

> 冇有自學能力的人冇有未來

**作者：李笑來**

特別感謝**霍炬**（[@virushuo](https://github.com/virushuo)）、**洪強甯**（[@hongqn](https://github.com/hongqn)) 兩位良師諍友在此書寫作過程中給予我的巨大幫助！

```python
# pseudo-code of selfteaching in Python

def teach_yourself(anything):
    while not create():
        learn()
        practice()
    return teach_yourself(another)

teach_yourself(coding)
```

> 有興趣幫忙的朋友，請先行閱讀 [如何使用 Pull Request 為這本書校對](02.proof-of-work.md)。

## 目錄

> - [01.preface（**前言**）](01.preface.md)
> - [02.proof-of-work（**如何證明你真的讀過這本書？**）](02.proof-of-work.md)
> - [Part.1.A.better.teachyourself（**為什麼一定要掌握自學能力？**）](Part.1.A.better.teachyourself.md)
> - [Part.1.B.why.start.from.learning.coding（**為什麼把編程當作自學的入口？**）](Part.1.B.why.start.from.learning.coding.md)
> - [Part.1.C.must.learn.sth.only.by.reading（**隻靠閱讀習得新技能**）](Part.1.C.must.learn.sth.only.by.reading.md)
> - [Part.1.D.preparation.for.reading（**開始閱讀前的一些準備**）](Part.1.D.preparation.for.reading.md)
> - [Part.1.E.1.entrance（**入口**）](Part.1.E.1.entrance.md)
> - [Part.1.E.2.values-and-their-operators（**值及其相應的運算**）](Part.1.E.2.values-and-their-operators.md)
> - [Part.1.E.3.controlflow（**流程控製**）](Part.1.E.3.controlflow.md)
> - [Part.1.E.4.functions（**函數**）](Part.1.E.4.functions.md)
> - [Part.1.E.5.strings（**字符串**）](Part.1.E.5.strings.md)
> - [Part.1.E.6.containers（**數據容器**）](Part.1.E.6.containers.md)
> - [Part.1.E.7.files（**文件**）](Part.1.E.7.files.md)
> - [Part.1.F.deal-with-forward-references（**如何從容應對含有過多 “過早引用” 的知識？**）](Part.1.F.deal-with-forward-references.md)
> - [Part.1.G.The-Python-Tutorial-local（**官方教程：The Python Tutorial**）](Part.1.G.The-Python-Tutorial-local.md)
> - [Part.2.A.clumsy-and-patience（**笨拙與耐心**）](Part.2.A.clumsy-and-patience.md)
> - [Part.2.B.deliberate-practicing（**刻意練習**）](Part.2.B.deliberate-practicing.md)
> - [Part.2.C.why-start-from-writing-functions（**為什麼從函數開始？**）](Part.2.C.why-start-from-writing-functions.md)
> - [Part.2.D.1-args（**關於參數（上）**）](Part.2.D.1-args.md)
> - [Part.2.D.2-aargs（**關於參數（下）**）](Part.2.D.2-aargs.md)
> - [Part.2.D.3-lambda（**化名與匿名**）](Part.2.D.3-lambda.md)
> - [Part.2.D.4-recursion（**遞歸函數**）](Part.2.D.4-recursion.md)
> - [Part.2.D.5-docstrings（**函數的文檔**）](Part.2.D.5-docstrings.md)
> - [Part.2.D.6-modules（**保存到文件的函數**）](Part.2.D.6-modules.md)
> - [Part.2.D.7-tdd（**測試驅動的開發**）](Part.2.D.7-tdd.md)
> - [Part.2.D.8-main（**可執行的 Python 文件**）](Part.2.D.8-main.md)
> - [Part.2.E.deliberate-thinking（**刻意思考**）](Part.2.E.deliberate-thinking.md)
> - [Part.3.A.conquering-difficulties（**戰勝難點**）](Part.3.A.conquering-difficulties.md)
> - [Part.3.B.1.classes-1（**類 —— 麵嚮對象編程**）](Part.3.B.1.classes-1.md)
> - [Part.3.B.2.classes-2（**類 —— Python 的實現**）](Part.3.B.2.classes-2.md)
> - [Part.3.B.3.decorator-iterator-generator（**函數工具**）](Part.3.B.3.decorator-iterator-generator.md)
> - [Part.3.B.4.regex（**正則錶達式**）](Part.3.B.4.regex.md)
> - [Part.3.B.5.bnf-ebnf-pebnf（**BNF 以及 EBNF**）](Part.3.B.5.bnf-ebnf-pebnf.md)
> - [Part.3.C.breaking-good-and-bad（**拆解**）](Part.3.C.breaking-good-and-bad.md)
> - [Part.3.D.indispensable-illusion（**剛需幻覺**）](Part.3.D.indispensable-illusion.md)
> - [Part.3.E.to-be-thorough（**全麵 —— 自學的境界**）](Part.3.E.to-be-thorough.md)
> - [Part.3.F.social-selfteaching（**自學者的社交**）](Part.3.F.social-selfteaching.md)
> - [Part.3.G.the-golden-age-and-google（**這是自學者的黃金時代**）](Part.3.G.the-golden-age-and-google.md)
> - [Part.3.H.prevent-focus-drifting（**避免註意力漂移**）](Part.3.H.prevent-focus-drifting.md)
> - [Q.good-communiation（**如何成為優秀溝通者**）](Q.good-communiation.md)
> - [R.finale（**自學者的終點**）](R.finale.md)
> - [S.whats-next（**下一步幹什麼？**）](S.whats-next.md)
> - [T-appendix.editor.vscode（**Visual Studio Code 的安裝與配置**）](T-appendix.editor.vscode.md)
> - [T-appendix.git-introduction（**Git 簡介**）](T-appendix.git-introduction.md)
> - [T-appendix.jupyter-installation-and-setup（**Jupyterlab 的安裝與配置**）](T-appendix.jupyter-installation-and-setup.md)
> - [T-appendix.symbols（**這些符號都代錶什麼？**）](T-appendix.symbols.md)

## 關於 `.ipynb` 文件轉換為 `.md` 文件的備註：

````bash
# 需提前安裝 nbconvert 插件，Terminal 下執行：
$ jupyter nbconvert --to markdown *.ipynb

而後將所有 `.md` 文件移到 `markdown/` 目錄之下 —— 除 `README.md` 文件之外

`README.md` 文件複製一份到 `markdown/` 目錄之下，而後編輯為當前文件

# 需使用 VSCode 批量 Find and Replace:
將所有 (https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/ 替換為 (https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/
將所有 (Part.1.A.better.teachyourself_files/ 替換為 (https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/
將所有 (Part.1.E.6.containers_files/ 替換為 (https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/
將所有 ```\n\n 替換為 ```\n
將所有	\n\n```	替換為 \n```
將所有 .ipynb) 替換為 .md)

`Part.1.E.3.controlflow.md` 文件中有過長的 output 需要編輯
`Part.1.E.7.files.md` 文件中有過長的 output 需要編輯
````

---

推薦讀者在自己的瀏覽器上安裝 [Stylus](https://github.com/openstyles/stylus) 這類終端 CSS 定製插件，Chrome/Firefox/Opera 都支持 Stylus 插件。以便擁有更好的閱讀體驗。以下 gif 圖片展示的是使用自定義 css 前後的效果：

> ![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/github-markdown-style.gif?raw=true)

我用的 Stylus 定製 CSS（針對 github.com）是這樣的：

```css
.markdown-body {font-family: "PingFang SC";}
strong {color:#6392BF;}
em {color: #A9312A; font-style: normal !important;}
table {font-size: 95% !important;}


.CodeMirror, pre {font-size: 90%;}
pre {
    padding: 10px 25px;
    background-color: #fafafa;
    border-left: 4px solid #dadada;
    border-radius: 10px;
}

pre code {
    background-color: #fafafa;
}

h1 code,
h2 code,
h3 code,
h4 code,
p code,
li code,
blockquote p code,
blockquote li code,
td code {
    background-color: #f6f6f6;
    font-size: 90%;
    color:#2e2e2e;
    padding: 4px 4px;
    margin: 0 8px;
    box-shadow: 0px 1px 2px 0px rgba(0,0,0,0.2);
    border-radius: 4px;
}
}
```

我寫的內容裏，為了重點突出，特別定製了 `strong` 和 `em` 兩個元素的顯示，讓它們以不同的顔色展示；又因為中文並不適合斜體展示，所以，把 `em` 的 `font-style` 設定為 `normal`……

---

本書的版權協議為 [CC-BY-NC-ND license](https://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)。

![CC-BY-NC-ND](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/CC-BY-NC-ND.png?raw=true)

---

**腳註**

<a name='fn1'>[1]</a>：['Themselves' or 'themself'?-- Oxford Dictionary](https://en.oxforddictionaries.com/usage/themselves-or-themself)

<a href='#fn1b'><small>↑Back to Content↑</small></a>
