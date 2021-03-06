# 如何從容應對含有過多 “過早引用” 的知識？

“過早引用”（[Forward References](https://en.wikipedia.org/wiki/Forward_declaration#id=Forward_reference)，另譯為 “前置引用”），原本是計算機領域的術語。

在幾乎所有的編程語言中，對於變量的使用，都有 “先聲明再使用” 的要求。直接使用未聲明的變量是被禁止的。Python 中，同樣如此。如果在從未給 `an_undefined_variable` 賦值的情況下，直接調用這個變量，比如，`print(an_undefined_variable)`，那就會報錯：`NameError: name 'an_undefined_variable' is not defined`。

```python
print(an_undefined_variable)
```

    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-1-7e0e1cc14e37> in <module>
    ----> 1 print(an_undefined_variable)

    NameError: name 'an_undefined_variable' is not defined

充滿過早引用的知識結構，在大腦中會構成類似 M.C. Escher 善畫的那種 “不可能圖形” 那樣的 “結構”。

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/four-cones.png?raw=true)

在上圖中，前三個椎形一般不會造成視覺睏惑 —— 尤其是第一個。

若是加上虛線，比如，第二個和第三個，那麼由於我們預設虛線錶示 “原本應該看不見的部分”，於是，`C` 點的位置相對於 `B` 和 `D` 應該更靠近自己；`C'` 的位置，相對於 `B'` 和 `D'` 應該更遠離自己……

然而，在第四個椎形中，由於 `B"D"` 和 `A"C"` 都是實線，於是，我們一下子就失去了判斷依據，不知道 `C"` 究竟是離自己更近還是更遠？

對一個點的位置睏惑，連帶著它與其它三個點之間的關係。可若那不是錐體，而是立方體呢？每個點的位置睏惑會造成對它與更多點之間的更多聯係的睏惑…… 若是更多麵體呢？

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/2_necker_cubes.png?raw=true)

把這些令人睏惑的點，比喻成 “過早引用”，你就明白為什麼 “很多過早引用” 的知識結構會那麼令人睏惑，處理起來那麼令人疲憊了吧？

## 過早引用就是無所不在

可生活、學習、工作，都不是計算機，它們可不管這套，管它是否定義過，管它是否定義清晰，直接甩出來就用的情況比比皆是。

對絕大多數 “不懂事” 的小朋友來說，幾乎所有痛苦的根源都來自這裏：“懂事” 的定義究竟是怎樣的呢？什麼樣算作懂事，什麼樣算作不懂事？弄不好，即便整個童年都在揣摩這個事，到最後還是迷迷糊糊。他們的父母，從未想過對孩子說話也好提要求也好，最好 “先聲明再使用”，或者即便事先聲明過也語焉不詳…… 於是，這些可憐的孩子，能做的隻有在惶恐中摸索，就好像在黑暗中拚圖一樣。

可事實上，他們的父母也不容易。因為確實有太多細節，給小朋友講了也冇用，或者講也講不清楚，又或者拚命解釋清楚了，但小朋友就是聽不進去…… 所以，令人惱火的 “過早引用”，有時候真的是隻能那樣的存在。

談戀愛的時候也是這樣。太多的概念，仟真萬確地屬於過早引用。愛情這東西究竟是什麼，剛開始的時候誰都弄不大明白。並且事實證明，身邊的絕大多數人跟自己一樣迷糊。至於從小說電影裏獲得的 “知識”，雖然自己看心神愉悅，但幾乎肯定給對方帶來無窮無盡的煩惱 —— 於對方來說你撒出來的是漫天飛舞的過早引用……

到了工作階段，技術崗位還相對好一點，其他領域，哪哪兒都是過早引用，並且還隱藏著不可見，搞得人們都弄出了一門玄學，叫做 “潛規則”。

人們歲數越大，交朋友越來越不容易。最簡單的解釋就是，每個人的曆史，對他人來說都構成 “過早引用”。所以，理解萬歲？太難了吧，幼兒園、小學的時候，人們之間幾乎不需要刻意相互理解，都冇覺得有這個必要；中學的時候，相互理解就已經開始出現不同程度的睏難了，因為過早引用的積纍。大學畢業之後，再工作上幾年，不僅相互理解變得越來越睏難，還有另外一層更大的壓力 —— 生活中要處理的事情越來越多，腦力消耗越來越大，遇到莫名其妙的過早引用，哪兒有心思處理？

## 不懂也要硬著頭皮讀完

這是事實：大多數難以掌握的技能都有這個特點。人們通常用 “學習麯線陡峭” 來形容這類知識，隻不過，這種形容隻限於形容而已，對學習冇有實際的幫助。麵對這樣的實際情況，有冇有一套有效的應對策略呢？

首先是要學會一個重要的技能：

> **讀不懂也要讀完，然後重複很多遍。**

這是最重要的起點。聽起來簡單，甚至有點莫名其妙 —— 但以後你就會越來越深刻地體會到，這麼簡單的策略，絕大多數人竟然不懂，也因此吃了很多很多虧。

充滿了過早引用的知識結構，就不可能是一遍就讀懂的。別說這種信息密度極高的複雜且重要的知識獲取了，哪怕你去看一部好電影，也要多刷幾遍才能徹底看懂，不是嘛？比如，Quentin Tarantino 導演的 [Pulp Fiction (1994)](https://www.imdb.com/title/tt0110912/)、David Fincher 導演的 [Fight Club (1999)](https://www.imdb.com/title/tt0137523/)、Christopher Nolan 導演的 [Inception (2010)](https://www.imdb.com/title/tt1375666/)、或者 Martin Scorsese 導演的 [Shutter Island (2010)](https://www.imdb.com/title/tt1130884/)……

所以，從一開始就要做好*將要重複很多遍*的準備，從一開始就要做好*第一次隻能讀懂個大概*的準備。

古人說，讀書百遍其義自見，道理就在這裏了 —— 隻不過，他們那時候冇有計算機術語可以借用，所以，這道理本身成了 “過早引用”，對那些根本就冇有過 “讀書百遍” 經曆的人，絕對以為那隻不過是在忽悠自己……

有經驗的讀書者，拿來一本書開始自學技能的時候，他會先翻翻目錄（Table Of Contents），看看其中有冇有自己完全冇有接觸過的概念；然後再翻翻術語錶（Glossary），看看是否可以盡量理解；而後會看看索引（Index），根據頁碼提示，直接翻到相關頁麵進一步查找…… 在通讀書籍之前，還會看看書後的參考文獻（References），看看此書都引用了哪些大牛的書籍，弄不好會順手多買幾本。

這樣做，顯然是老到 —— 這麼做的最大好處是 “盡力消解了大量的過早引用”，為自己減少了極大的理解負擔。

所以，第一遍的正經手段是 “**囫圇吞棗**地讀完”。

囫圇吞棗從一開始就是貶義詞。但在當前這個特殊的情況下，它是最好的策略。那些隻習慣於一上來就仔細認真的人，在這裏很吃虧，因為他們越是仔細認真，越是容易被各種過早引用搞得灰心喪氣；相應地，他們的挫敗感積纍得越快；到最後弄不好最先放棄的是他們 —— 失敗的原因竟然是因為 “太仔細了”……

第一遍囫圇吞棗，用個正麵一點的描述，就是 “_為探索未知領域先畫個潦草的地圖_”。地圖這東西，有總比冇有好；雖然說它最好精確，但即便是 “不精確的地圖” 也比 “完全冇地圖” 好一萬倍，對吧？更何況，這地圖總是可以不斷校正的，不是嗎？世界上哪個地圖不是一點一點校正過來才變成今天這般精確的呢？

## 磨練 “隻字不差” 的能力

通過閱讀習得新技能（尤其是 “盡量隻通過閱讀習得新技能”），肯定與 “通過閱讀獲得心靈愉悅” 很不相同。

讀個段子、讀個小說，讀個當前熱搜文章，通常情況下不需要 “精讀” —— 草草瀏覽已經足夠，頂多對自己特別感興趣的地方，慢下來仔細看看……

但是，若是為了習得新技能去閱讀，就要施展 “**隻字不差地閱讀**” 這項專門的技能。

對，“隻字不差地閱讀” 是所有自學能力強的人都會且都經常使用的技能。尤其是當你在閱讀一個重要概念的定義之時，你就是這麼幹的：定義中的每個字都是有用的，每個詞的內涵外延都是需要進行推敲的，它是什麼，它不是什麼，它的內涵外延都是什麼，因此，在使用的時候需要註意什麼……

很有趣的一個現象是，絕大多數自學能力差的人，都是把一切都當作小說去看，隨便看看，粗略看看……

你有冇有註意到一個現象，人們在看電影的時候，絕大多數人會錯過絕大多數細節；但這好像並不會削減他們的觀影體驗；並且，他們有能力使用錯過了無數細節之後剩下的那些碎片拚接出一個 “完整的故事” —— 當然，通常幹脆是 “另一個貌似完整的故事”。於是，當你在跟他們討論同一個電影的時候，常常像是你們冇坐在同一個電影院，看的不是同一個電影似的……

所謂的自學能力差，很可能最重要的坑就在這裏：

> 每一次學習新技能的時候，很多人隻不過是因為做不到隻字不差地閱讀，於是總是會錯過很多細節；於是，最終就好像 “看了另外一個山寨版電影一樣”，實際上 “習得了另外一個山寨版技能”……

在學習 Python 語言的過程中，有個例子可以說明以上的現象。

在 Python 語言中，`for` 循環可以附加一個 `else` 部分。你到 Google 上搜索一下 [`for else python`](https://www.google.com/search?q=for+else+python) 就能看到有多少人在 “追問” 這是幹什麼的？還有另外一些鏈接，會告訴你 “for... else” 這個 “秘密” 的含義，將其稱為 “語法糖” 什麼的……

其實，[官方教程](https://docs.python.org/3/tutorial/controlflow.html#break-and-continue-statements-and-else-clauses-on-loops)裏寫的非常清楚的，並且還給出了一個例子：

> Loop statements may have an else clause; it is executed when the loop terminates through exhaustion of the list (with for) or when the condition becomes false (with while), but not when the loop is terminated by a break statement. This is exemplified by the following loop, which searches for prime numbers:
>
> ```python
> >>> for n in range(2, 10):
> ...     for x in range(2, n):
> ...         if n % x == 0:
> ...             print(n, 'equals', x, '*', n//x)
> ...             break
> ...     else:
> ...         # loop fell through without finding a factor
> ...         print(n, 'is a prime number')
> ...
> 2 is a prime number
> 3 is a prime number
> 4 equals 2 * 2
> 5 is a prime number
> 6 equals 2 * 3
> 7 is a prime number
> 8 equals 2 * 4
> 9 equals 3 * 3
> ```

隻有兩種情況，

> - 要麼幹脆就冇讀過，
> - 要麼是讀了，卻冇讀到這個細節……

—— 後者更為可怕，跟花了同樣的錢看了另外一個殘缺版本的電影似的……

為什麼說 “隻字不差地閱讀” 是一項專門的技能呢？你自己試過就知道了。明明你已經刻意讓自己慢下來，也刻意揣摩每個字每個詞的含義，甚至為了理解正確，做了很多筆記…… 可是，當你再一次 “隻字不差地閱讀” 的時候，你經常會 “驚訝地發現”，自己竟然有若幹處遺漏的地方！對，這就是一種需要多次練習、長期訓練才能真正掌握的技能。絕對不像聽起來那麼簡單。

所以，_到了第二遍第三遍就必須施展 “隻字不差地閱讀” 這項專門的技能了_，隻此一點，你就已然**與衆不同**了。

## 好的記憶力很重要

“就算讀不懂也要讀完” 的更高境界，是 “**就算不明白也要先記住**”。

人們普遍討厭 “死記硬背”…… 不過，說實話，這很膚淺。雖然確實也有 “擅長死記硬背卻就是什麼都不會的人”，但是，其實有更多記憶力強的人，實際上更可能是 “博聞強識”。

麵對 “過早引用” 常見的知識領域，好記憶力是超強加分項。記不清、記不住、甚至幹脆忘了 —— 這是自學過程中最耽誤事的缺點。尤其在有 “過早引用知識點” 存在的時候，更是如此。

然而，很多人並冇有意識到的是，記憶力也是 “一門手藝” 而已。並且，事實上，它是任何時候都可以通過刻意練習加強的 “手藝”。

更為重要的是，記憶力這個東西，有一百種方法去彌補 —— 比如，最明顯、最簡單的辦法就是 “好記性不如爛筆頭”……

所以，在絕大多數正常情況下，所謂的 “記不清、記不住、甚至幹脆忘了”，都隻不過是懶的結果 —— 若是一個人懶，且不肯承認自己懶，又因為不肯承認而已就不去糾正，那…… 那就算了，那就那麼活下去罷。

然而，提高對有效知識的記憶力還有另外一個簡單實用的方法 —— 而市麵上有各種 “快速記憶法”，通常相對於這個方法來看用處並不大。

這個方法就是以下要講到的 “整理歸納總結” —— **反複做整理歸納總結，記不住才怪呢！**

## 盡快開始整理歸納總結

從另外一個角度，這類體係的知識書籍，對作者來說，不僅是挑戰，還是擺脫不了的負擔。

Python 官方網站上的 [The Python Tutorial](https://docs.python.org/3/tutorial/index.html)，是公認的最好的 Python 教材 —— 因為那是 Python 語言的作者 [Guido van Rossum](https://en.wikipedia.org/wiki/Guido_van_Rossum) 寫的……

雖然 Guido van Rossum 已經很小心了，但還是冇辦法在講解上避免大量的過早引用。他的小心體現在，在目錄裏就出現過五次 **More**：

> - More Control Flow Tools
> - More on Defining Functions
> - More on Lists
> - More on Conditions
> - More on Modules

好幾次，他都是先粗略講過，而後在另外一處再重新深入一遍…… 這顯然是一個最盡力的作者了 —— 無論是在創造一個編程語言上，還是在寫一本教程上。

然而，即便如此，這本書對任何初學者來說，都很難。當個好作者不容易。

於是，這隻能是讀者自己的工作了 —— 因為即便是最牛的作者，也隻能到這一步了。

第一遍囫圇吞棗之後，馬上就要開始 “**總結**、**歸納**、**整理**、**組織** 關鍵知識點” 的工作。自己動手完成這些工作，是所謂學霸的特點。他們隻不過是掌握了這樣一個其他人從未想過必須掌握的簡單技巧。他們一定有個本子，裏麵是各種*列錶*、_示意圖_、_錶格_ —— 這些都是最常用的知識（概念）整理組織歸納工具，這些工具的用法看起來簡單的要死。

這個技巧說出來、看起來都非常簡單。然而，也許正因為它看起來如此簡單，才被絕大多數人忽略…… 與學霸們相對，絕大多數非學霸都有一模一樣的糊弄自己的理由：反正有別人做好的，拿過來用就是了！—— 聽起來那麼理直氣壯……

可實際上，**自己動手做做就知道了** —— 整理、歸納、組織，再次反複，是個相當麻煩的過程。非學霸們自己不動手做的真正原因隻不過是：嫌麻煩、怕麻煩。一個字總結，就是，**懶**！可是，誰願意承認自己懶呢？冇有人願意。於是，都給自己找個冠冕堂皇的理由，比如，上麵說的 “反正別人已經做好了，我為什麼還要再做一遍呢？” 再比如，“這世界就是懶人推進的！”

久而久之，各種愛麵子的說法完美地達成了自我欺騙的效果，最後連自己都信了！於是，身上多了一個明明存在卻永遠找不到的漏洞 —— **且不自知**。

我在第一次粗略讀過整個 [Python Official Tutorial](https://docs.python.org/3/tutorial/datastructures.html) 中的第五章之後，順手整理了一下 Containers 的概念錶格：

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/python-containers.png?raw=true)

**可這張圖錯了！**

因為我最早 “合理囫圇吞棗” 的時候，`Bytes` 這種數據類型全部跳過；而後來多輪反複之後繼續深入，又去讀 [The Python Language Reference](https://docs.python.org/3/reference/datamodel.html) 的第五章 `Data Model` 之後，`發現 Set` 也有 Immutable，是 `Frozen Set`…… 當然，最錯的是，整理的過程中，一不小心把 “Ordered” 給弄反了！

於是肯定需要再次整理，若幹次改進之後，那張圖就變成了下麵這個樣子：

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/python-containers-final.png?raw=true)

> 另外，從 Python 3.7 開始，Dictionary 是 insertion ordered 了：<br />
> https://docs.python.org/3/library/collections.html#ordereddict-objects

這個自己動手的過程其實真的 “很麻煩”，但它實際上是幫助自己強化記憶的過程，並且對自我記憶強化來說，絕對是不可或缺的過程。習慣於自己動手做罷！習慣於自己不斷修改罷！

再給你看個善於學習的人的例子：

> https://nvie.com/posts/iterators-vs-generators/

作者 Vincent Driessen 在這個帖子裏寫到：

> I'm writing this post as a pocket reference for later.

人家隨手做個圖，都捨不得不精緻：

![](https://raw.githubusercontent.com/selfteaching/the-craft-of-selfteaching/master/images/iter-relationships.gif?raw=true)

自學能力強的人有個特點，就是**不怕麻煩**。小時候經常聽到母親念叨，“怕麻煩！那還活著幹嘛啊？活著多麻煩啊！” —— 深刻。

## 先關註使用再研究原理

作為人類，我們原本很擅長運用自己並不真正理解的物件、技能、原理、知識的……

三仟多年以前，一艘歐洲腓尼基人的商船在貝魯斯河上航行的時候擱淺了…… 於是，船員們紛紛登上沙灘。餓了怎麼辦？架火做飯唄。吃完飯，船員們驚訝地發現鍋下麵的沙地上有很多亮晶晶、閃閃發光的東西！今天的化學知識對當年的他們來說，是那一生不可觸摸的 “過早引用”。他們並不懂這個東西的本質、原理，但稍加研究，他們發現的是，鍋底沾有他們運輸的天然蘇打…… 於是，他們的總結是，天然蘇打和沙子（我們現在知道沙子中含有石英砂）被火燒，可能會産生這個東西。幾經實驗，成功了。於是，腓尼基人學會了製做玻璃球，發了大財……

兩仟五六百年之前，釋加牟尼用他的理解以及在那個時代有限的概念詳細敘述了打坐的感受 —— 他曾連續打坐 6 年。今天，西方科學家們在深入研究腦科學的時候，發現 [Meditation](https://en.wikipedia.org/wiki/Meditation) 對大腦有特別多的好處…… 這些好處就是好處，與宗教全然冇有任何關係的好處。

> - [Harvard neuroscientist: Meditation not only reduces stress, here's how it changes your brain](https://www.washingtonpost.com/news/inspired-life/wp/2015/05/26/harvard-neuroscientist-meditation-not-only-reduces-stress-it-literally-changes-your-brain/)
> - [This Is Your Brain on Meditation -- The science explaining why you should meditate every day](https://www.psychologytoday.com/us/blog/use-your-mind-change-your-brain/201305/is-your-brain-meditation)
> - [Researchers study how it seems to change the brain in depressed patients](https://news.harvard.edu/gazette/story/2018/04/harvard-researchers-study-how-mindfulness-may-change-the-brain-in-depressed-patients/)
> - [Meditation's Calming Effects Pinpointed in the Brain](https://www.scientificamerican.com/article/meditations-calming-effects-pinpointed-in-brain/)
> - [Different meditation types train distinct parts of your brain](https://www.newscientist.com/article/2149489-different-meditation-types-train-distinct-parts-of-your-brain/)

你看，我們原本就是可以直接使用自己並不真正理解的物件、技能、原理、知識的！可為什麼後來就不行了呢？

或者說，從什麼時候開始，我們開始害怕自己並不真正理解的東西，不敢去用，甚至連試都不敢去試了呢？

有一個相當惱人的解釋：**上學上壞了**。

學校裏教的全都是屬於 “先聲明再使用” 的知識。反過來，不屬於這種體係架構的知識，學校總是回避的 —— 比如，關於投資與交易的課程，從來看不見地球上有哪個義務教育體係把它納入教學範圍。雖然，投資與交易，是每個人都應該掌握、都必須掌握的不可或缺的技能，某種意義上它甚至比數學語文都更重要，然而，學校就是不會真教這樣的東西。

而且，現在的人上學的時間越來越長。小學、初中、高中、本科加起來 16 年…… 這麼長時間的 “熏陶”，隻能給大多數人造成幻覺，嚴重、深刻，甚至不可磨滅的幻覺，誤以為所有的知識都是這種類型…… 可偏偏，這世界上真正有用的、真正必要的知識，幾乎全都不是這種類型 —— 頗令人惱火。

現在的你，不一樣了 —— 你要跳出來。養成一個習慣：

> 不管怎麼樣，先用起來，反正，研究透原理，不可能馬上做到，需要時間漫漫。

用錯了冇關係，改正就好。用得不好冇關係，用多了就會好。隻要開始用起來，理解速度就會加快 —— 實踐出真知，不是空話。

有的時候，就是因為冇有犯過錯，所以不可能有機會改正，於是，就從未做對過。

## 尊重前人的總結和建議

生活中，年輕人最常犯的錯誤就是把那句話當作屁：

> 不聽老人言，吃虧在眼前。

對年輕人來講，老人言確實很討厭，尤其是與自己當下的感受相左的時候。

然而，這種 “討厭” 的感覺，更多的時候是陷阱，因為那些老人言隻不過是過早引用，所以，在年輕人的腦子裏 “無法執行”，“報錯為類型錯誤”……

於是，很多人一不小心就把 “不聽老人言” 和 “獨立思考” 混淆起來，然後最終自己吃了虧。可尷尬在於，等自己意識到自己吃虧了的時候吧，大量的時間早已飄逝，是為 “無力回天”。

你可以觀察到一個現象，學霸（好學生）的特點之一就是 “老師讓幹啥就幹啥”，冇廢話。

比如，上麵告訴你了，“必須自己動手”，那你就從現在開始老老實實地在一切必要的情況下自己動手去 “**總結**、**歸納**、**整理**、**組織** 關鍵知識點”…… 那你就必然能夠學好。但針對這麼個建議，你反複在那裏問，“為什麼呀？”，“有冇有更簡單的辦法啊？”…… 那你就完了，死定了。

學寫代碼的過程中，有很多重要的東西實際上並不屬於 “編程語言範疇”。比如，如何為變量命名、如何組織代碼，這些 “規範”，不是違背了就會馬上死掉的<a href='#fn1' name='fn1b'><sup>[1]</sup></a>；並且，初來乍到的時候，這些東西看起來就是很囉嗦、很麻煩的…… 然而，這些東西若是不遵守，甚至幹脆不了解，那麼最終的結果是，你永遠不可能寫出大項目，永遠是小打小鬨 —— 至於為什麼，可以用那句你最討厭的話回答你：

> 等你長大了就懂了……

自學編程的好處之一，就是有機會讓一個人見識到 “規範”、“建議” 的好處。也有機會讓一個人見識到不遵守這些東西會吃怎樣的虧（往往是現世報）。

Python 中有一個概念叫 PEP，Python Enhancement Proposals，必須找時間閱讀，反複閱讀，牢記於心：

> https://www.python.org/dev/peps/pep-0008/

到最後，你會體會到，這不隻是編程的事，這種東西背後的思考與體量，對整個人生都有巨大幫助。

---

**腳註**

<a name='fn1'>[1]</a>：也可能真的會死…… 請看一篇 2018 年 9 月份的一則新聞，發生在舊金山的事情：[Developer goes rogue, shoots four colleagues at ERP code maker](https://www.theregister.co.uk/2018/09/20/developer_work_shooting/)

<a href='#fn1b'><small>↑Back to Content↑</small></a>
