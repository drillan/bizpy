---
title: 企業の財務データを可視化しよう
tags: Python
description: ビジネスパーソンの日常業務で Python を活用する人のための勉強会
slideOptions:
  spotlight:
    enabled: true
  allottedMinutes: 10  # Minutes alloted for a slide.
---

# 企業の財務データを可視化しよう

ビジネスPythonを学ぶ会
2020-11-11

driller[@patraqushe](https://twitter.com/patraqushe)

----

### 誰？

- [どりらん](https://twitter.com/patraqushe) ![](https://i.imgur.com/u7l3rnc.png)
- [fin-py](https://fin-py.connpass.com)
- ぼっち会社経営
    - 在宅勤務歴10年
    - 非エンジニア
- よく歩いてます<a href="https://www.dragonquest.jp/walk/"><img src="https://pbs.twimg.com/profile_images/1169446429720363008/EAQDTMsd.png" width=35 height=35></a>

----

### fin-py

Python × 金融のコミュニティ

![](https://github.com/fin-py/logo/blob/master/finpy_background_200x200.png?raw=true)

----

#### [fin-pyもくもく会 #38](https://fin-py.connpass.com/event/186842/)

https://fin-py.connpass.com/event/193937/

- オンライン(Discord)のもくもく会
- 2020/11/14(土) 10:00 〜 13:00

----

#### 共著1

Pythonインタラクティブ・データビジュアライゼーション入門  
―Plotly/Dashによるデータ可視化とWebアプリ構築―  

[![](https://github.com/drillan/bizpy/blob/main/20201111/assets/plotly-dash-book-cover.png?raw=true)](https://amzn.to/38vKE1g)

----

#### 共著2

改訂版 Pythonユーザのための Jupyter［実践］入門  

[![jupyterbook](https://gihyo.jp/assets/images/cover/2020/thumb/TH160_9784297115685.jpg)](https://amzn.to/3khPFwr)

----

#### 雑誌

2018年2月号|SD別冊シリーズ|2019年4月号|2020年2月号|2020年10月号
---|---|---|---|---
[![](https://gihyo.jp/assets/images/cover/2018/thumb/TH160_641802.jpg)](https://gihyo.jp/magazine/SD/archive/2018/201802)|[![](https://gihyo.jp/assets/images/cover/2019/thumb/TH160_9784297103965.jpg)](https://gihyo.jp/book/2019/978-4-297-10396-5)|[![](https://gihyo.jp/assets/images/cover/2019/thumb/TH160_641904.jpg)](https://gihyo.jp/magazine/SD/archive/2019/201904)|[![](https://gihyo.jp/assets/images/cover/2020/thumb/TH160_642002.jpg)](https://gihyo.jp/magazine/SD/archive/2020/202002)|[![](https://gihyo.jp/assets/images/cover/2020/thumb/TH160_642010.jpg)](https://gihyo.jp/magazine/SD/archive/2020/202010)

---

### 今回のテーマ

財務データを可視化しよう

----

#### 財務諸表

> 財務諸表（ざいむしょひょう、financial statements）は、企業が利害関係者に対して一定期間の経営成績や財務状態等を明らかにするために複式簿記に基づき作成される書類である。日常用語としては、決算書（又は決算報告書）と呼ばれている。

「財務諸表」（2020年10月20日 (火) 04:19　UTCの版）『ウィキペディア日本語版』。

https://ja.wikipedia.org/wiki/財務諸表

----

#### 財務諸表の理解が必要なロール

- 経営者
- 経理関係者
- 金融関係者

----

#### すべてビジネスパーソンに有効

- 自社・他社(競合・転職先・就職先)の把握・分析
    - 将来性・成長性
    - 経営の健全性・持続性
- マクロ環境の影響
    - 金利
    - 株価

----

#### 財務諸表を可視化することで得られる情報

- 時系列の推移
- 複数企業の比較
- 分布
- 内訳の把握

----

#### 今回まなぶこと

- [Colabratory](colab.research.google.com/) の簡単な使い方
- [pandas](https://pandas.pydata.org) によるデータ処理
- [Plotly Express(plotly.py)](https://plotly.com/python/) によるインタラクティブな可視化