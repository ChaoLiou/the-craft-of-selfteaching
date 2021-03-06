# 類 —— 麵嚮對象編程

## 麵嚮對象編程

註意：當前這一小節所論述的內容，不是專屬於哪個編程語言（比如 Python、JavaScript 或者 Golang）。

麵嚮對象編程（[Object Oriented Programming, OOP](https://en.wikipedia.org/wiki/Object-oriented_programming)）是一種編程的範式（Paradigm），或者說，是一種方法論（Methodology）—— 可以說這是個很偉大的方法論，在我看來，現代軟件工程能做那麼複雜的宏偉項目，基本上都得益於這個方法論的普及。

## 爭議

現在，OOP 的支持者與反對者在數量上肯定不是一個等級，絕大多數人支持 OOP 這種編程範式。

但是，從另外一個角度，反對 OOP 的人群中，牛人比例更高 —— 這也是個看起來頗為吊詭的事實。

比如，Erlang 的發明者，[Joe Armstrong](<https://en.wikipedia.org/wiki/Joe_Armstrong_(programmer)>) 就很討厭 OOP，覺得它效率低下。他用的類比也確實令人忍俊不禁，說得也挺準的：

> 支持 OOP 的語言的問題在於，它們總是隨身攜帶著一堆並不明確的環境 —— 你明明隻不過想要個香蕉，可你所獲得的是一個大猩猩手裏拿著香蕉…… 以及那大猩猩身後的整個叢林！<br /> —— [Coders at Work](http://www.codersatwork.com)

創作 UTF-8 和 Golang 的程序員 [Rob Pike](https://en.wikipedia.org/wiki/Rob_Pike)，更看不上 OOP，在 2004 年的一個討論帖裏直接把 OOP 比作 “[Roman numerals of computing](https://groups.google.com/forum/#!topic/comp.os.plan9/VUUznNK2t4Q%5B151-175%5D)” —— 諷刺它就是很土很低效的東西。八年後又[挖墳把一個 Java 教授寫的 OOP 文章嘲弄了一番](https://plus.google.com/+RobPikeTheHuman/posts/hoJdanihKwb)：“也不知道是什麼腦子，認為寫 6 個新的 Class 比直接用 1 行錶格搜索更好？”

[Paul Graham](https://en.wikipedia.org/wiki/Paul_Graham_(programmer) —— 就是那個著名的 Y-Combinator 的創始人 —— 也一樣對 OOP 不以為然，在 [Why Arc isn't Especially Object-Oriented](http://www.paulgraham.com/noop.html) 中，說他認為 OOP 之所以流行，就是因為平庸程序員（Mediocre programers）太多，大公司用這種編程範式去阻止那幫家夥，讓他們捅不出太大的婁子……

然而，爭議歸爭議，應用歸應用 —— 就好像英語的弊端不見得比其他語言少，可就是最流行，那怎麼辦呢？用唄 —— 雖然該抱怨的時候也得抱怨抱怨。

從另外一個角度望過去，大牛們如此評價 OOP 也是很容易理解的 —— 因為他們太聰明，又因為他們太懶得花時間去理解或容忍笨蛋…… 我們不一樣，最不一樣的地方在於，我們不僅更多容忍他人，而且更能夠容忍自己的愚笨，所以，視角就不同了，僅此而已。

並且，上麵兩位大牛寫的編程語言，現在也挺流行，Joe Armstrong 的 Erlang 和 Rob Pike 的 Golang，弄不好早晚你也得去學學，去用用……

## 基本術語

麵嚮對象編程（OOP），是使用**對象**（Objects）作為核心的編程方式。進而就可以把對象（Objects）的數據和運算過程**封裝**（Encapsulate）在內部，而外部僅能根據事先設計好的**界麵**（Interface）與之溝通。

比如，你可以把燈泡想象成一個對象，使用*燈泡*的人，隻需要與*開關*這個界麵（Interface）打交道，而不必關心燈泡內部的設計和原理 —— 說實話，這是個很偉大的設計思想。

生活中，我們會遇到無數有意無意應用了這種設計思想的産品 —— 並不僅限於編程領域。你去買個車回來，它也一樣是各種封裝之後的對象。當你轉動方嚮盤（操作界麵）的時候，你並不需要關心汽車設計者是如何做到把那個方嚮盤和車輪車軸聯係在一起並如你所願去轉嚮的；你隻需要知道的是，逆時針轉動方嚮盤是左轉，而順時針轉動方嚮盤是右轉 —— 這就可以了！

在程序設計過程中，我們常常需要對標現實世界創造對象。這時候我們用的最直接手段就是**抽象**（Abstract）。抽象這個手段，在現實中漫畫家們最常用。為什麼你看到下麵的圖片覺得它們倆看起來像是人？尤其是在你明明知道那肯定不是人的情況下，卻已然接受那是兩個漫畫小人的形象？

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/a-cartoon.png?raw=true)

這種描繪方式，就是抽象，很多 “冇必要” 的細節都被去掉了（或者反過來說，冇有被採用），留下的兩個特徵，一個是頭，一個是雙眼 —— 連那雙 “眼睛” 都抽象到隻剩下一個黑點了……

這種被保留下來的 “必要的特徵”，叫做對象的**屬性**（Attributes），進而，這些抽象的對象，既然是 “人” 的映射，它們實際上也能做一些抽象過後被保留下來的 “必要的行為”，比如，說話，哭笑，這些叫做對象的**方法**（Methods）。

從用編程語言創造對象的角度去看，所謂的界麵，就由這兩樣東西構成：

> - _屬性_ —— 用自然語言描述，通常是名詞（Nouns）
> - _方法_ —— 用自然語言描述，通常是動詞（Verbs）

從另外一個方麵來看，在設計複雜對象的時候，抽象到極緻是一種必要。

我們為生物分類，就是一層又一層地抽象的過程。當我們使用 “生物” 這個詞的時候，它並不是某一個特定的我們能夠指稱的東西…… 然後我們開始給它分類……

[![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/Tree-of-Life.gif?raw=true)](https://crucialconsiderations.org/wp-content/uploads/2016/08/Tree-of-Life.jpg)

所以，當我們在程序裏創建對象的時候，做法常常是

> - 先創建最抽象的**類**（Class）
> - 然後再創建**子類**（Subclass）……

它們之間是從屬關係是：

> Class ⊃ Subclass

在 OOP 中，這叫**繼承**（Inheritance）關係。比如，狗這個*對象*，就可以是從哺乳動物這個對象*繼承*過來的。如果哺乳動物有 “頭” 這個*屬性*（Attributes），那麼在狗這個對象中就冇必要再重新定義這個屬性了，因為既然狗是從哺乳動物繼承過來的，那麼它就擁有哺乳動物的所有屬性……

每當我們創建好一個類之後，我們就可以根據它創建它的許多個**實例**（Instances）。比如，創建好了 “狗” 這個類之後，我們就可以根據這個類創建很多條狗…… 這好多條狗，就是狗這個類的*實例*。

現在能把這些術語全部關聯起來了嗎？

> - 對象，封裝，抽象
> - 界麵，屬性，方法
> - 繼承，類，子類，實例

這些就是關於 “麵嚮對象編程” 方法論的最基本的術語 —— 無論在哪種編程語言裏，你都會頻繁地遇到它們。

**對象**、**類**，這兩個詞，給人的感覺是經常被通用 —— 習慣了還好，但對有些初學者來說，就感覺那是生命不能承受之重。—— 這次不是英文翻譯中文時出現的問題，在英文世界裏，這些詞的互通使用和濫用也使相當一部分人（我懷疑是大部分人）最終掌握不了 OOP 這個方法論。

細微的差異在於 “視角” 的不同。

之前提到函數的時候，我用的說辭是，

> - 你寫了一個函數，而後你要為這個産品的使用者寫說明書……
> - —— 當然，産品使用者之中也包括未來的你……

類（Class）這個東西也一樣，它也有創作者和使用者。

你可以這樣分步理解：

> - 你創造了一個類（Class），這時候你是創作者，從你眼裏望過去，那就是個類（Class）；
> - 而後你根據這個類的定義，創建了很多實例（Instances）；
> - 接下來一旦你開始使用這些實例的時候，你就成了使用者，從使用者角度望過去，手裏正在操作的，就是各種對象（Objects）……

最後，補充一下，不要誤以為所有的 Classes 都是對事物（即，名詞）的映射 —— 雖然大多數情況下確實如此。

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/code-review.png?raw=true)

對基本概念有了一定的了解之後，再去看 Python 語言是如何實現的，就感覺冇那麼難了。
