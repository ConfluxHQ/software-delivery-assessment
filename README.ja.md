# Multi-team Software Delivery Assessment

Multi-team Software Delivery Assessmentは、組織内のさまざまなチームのソフトウェア・デリバリーを評価するためのシンプルで実行しやすい手法です。    　　　　

この評価手法は、よく知られ実績のある[Spotify Squad Health Check model](https://labs.spotify.com/2014/09/16/squad-health-check-model/)を基にしており、以下、合計6つの観点をカバーしています。     

1. [Team Health](team-health.ja.md)
2. [Deployment](deployment.ja.md)
3. [Flow](flow.ja.md)
4. [Continuous Delivery](continuous-delivery.ja.md)
5. [Operability](operability.ja.md)
6. [Testing and Testability](testability.ja.md)

これらの6つの観点は、最新のソフトウェア・デリバリーのすべての重要事項を網羅していて、チームがそれぞれの長所とプラクティスを自己評価できます。            

**🚀 概要**: [Continuous Delivery at scale](https://www.slideshare.net/matthewskelton/continuous-delivery-at-scale-matthew-skelton-nhs-digital-agile-cop-march-2019)のスライド32〜38を参照してください。    

> Copyright © 2018-2019 [Conflux Digital Ltd](https://confluxdigital.net/)
> 
> Licenced under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) ![CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/3.0/88x31.png)
>
> _Permalink: [SoftwareDeliveryAssessment.com](http://SoftwareDeliveryAssessment.com/)_

## 評価の目的      

ソフトウェアシステムを構築および実行するためのポジティブな作業環境を促進および維持することが、評価の目的です。      
ポジティブな作業環境は以下の状況になります。       

  - ソフトウェアの変更は、継続的デリバリーの手法を使用して、**迅速かつ安全に**ビルドされ、テストされ、プロダクション環境にリリースされる。    
  - プロセスとプラクティスは、**リリースに向けたソフトウェアの変更フロー**に最適化される。         
  - ソフトウェアは、1つ１つ分断されたシステムに対して**独立、分離したリリース**ができるように設計および構築される。     
  - ソフトウェアは、**運用性**、**テスト容易性**、および**リリース容易性**を考慮して設計および構築される。    
  - ソフトウェアプロダクト、ソフトウェア生産過程での問題が、顧客やユーザーが気付く前に、常に**チームによって検出される**。     
  - 開発者がソフトウェアの変更に対する責任と**説明責任**を持つことは、開発者のエンパワーメントとオーナーシップに繋がる。     
  - ソフトウェア開発が、**やりがいのあり**、楽しいものになる。    
  - **悪い慣習と、悪いアプローチに挑み変えること** に自信が持てるようになる。        
 
基本的に、Multi-team Software Delivery Assessmentは**チームを解放して活性化**し、チームが成功するのに役立ちます。 この評価手法は、様々な改善点を特定することにより、**チームがソフトウェアシステムの構築、テスト、およびリリースを改善する**のを手助けします。       
改善点には、以下があります。      

1.チーム中心の改善点       
2.製品中心およびサービス中心の改善点     
3.組織全体の改善点            

この評価手法は、チームにペナルティを科すために使用するべきではなく、プラクティスと品質の改善に向けて、共有される意欲を提供するために使用するべきです。     

## 評価対象のチーム       

アプリケーションソフトウェアまたはインフラストラクチャのコード作成、スクリプト作成、またはコード設定、スクリプト設定を行うすべてのチームが評価対象となり、評価することでメリットがあります。            
評価対象のチームには以下があります。      

  - **ユーザー向け-のWebサイトとサービス**、**顧客向けのWebサイトとサービス**を構築するチーム       
  - **内部サービス**を構築するチーム      
  - 他のシステムをサポートする**インフラストラクチャ**を構築するチーム（プラットフォームチームを含む）        
  - **ビルド とデプロイメント**ツール、スクリプトを構築するチーム     
  - ソフトウェアおよびインフラストラクチャの一部としてCOTS製品を構成およびテストするチーム     
  - その他の、**ソフトウェアおよびインフラストラクチャの構築、構成、およびテスト** に主眼をおくチーム    
  
"チーム"とは、人材連携の度合いの大きいを6-10人のグループを意味します。通常、**Squad**、**Scrumチーム**、**Productチーム**、または **Stream-alignedチーム**と呼ばれます。

## 評価基準    

各観点の評価基準は、既存の出版された書籍およびオンラインソースから取得しています。     

* **Team Health** - [_Spotify Squad Health Check_](https://labs.spotify.com/2014/09/16/squad-health-check-model/) の評価基準に基づきながらいくつかのチェック項目を追加した。     
* **Deployment** - Mirco氏のブログ投稿[_DevOps for the Modern Enterprise_](https://itrevolution.com/book/devops_modern_enterprise/) で説明されている書籍[_DevOps for the Modern Enterprise_](https://itrevolution.com/book/devops_modern_enterprise/) の主要な質問に基づいている。     
* **Flow** - Nicole Forsgren氏、Jez Humble氏、Gene Kim氏の書籍  [_Accelerate_](https://itrevolution.com/book/accelerate/) の評価基準に基づきながら、Don Reinertsen 氏の書籍 [_The Principles of Product Development Flow_](https://www.amazon.com/Principles-Product-Development-Flow-Generation/dp/1935401009) から、いくつかチェック項目を追加した。    
* **Contous Delivery** - Jez Humble氏とDave Farley氏による書籍 [_Continuous Delivery_](https://www.amazon.com/Continuous-Delivery-Deployment-Automation-Addison-Wesley/dp/0321601912) と [CDchecklist.info](http://CDchecklist.info/) にある書籍の要約に基づいて作成した。     
* **Operability** - [OperabilityQuestions.com](http://OperabilityQuestions.com/)からの質問と、Matthew Skelton氏、Alex Moore氏、およびRob Thatcher氏による書籍[_Team Guide to Software Operability_](http://operabilitybook.com/) から選択した評価基準に基づいて作成した。       
* **Testing and Testability** - Lisa Crispin氏 と Janet Gregory氏による書籍 [_Agile Testing_](https://wordery.com/agile-testing-lisa-crispin-9780321534460) , Jez Humble氏とDave Farley氏による書籍 [_Continuous Delivery_](https://www.amazon.com/Continuous-Delivery-Deployment-Automation-Addison-Wesley/dp/0321601912) , Steve Freeman 氏 と Nat Price 氏 による書籍[_Growing Object-Oriented Software_](https://wordery.com/growing-object-oriented-software-guided-by-tests-steve-freeman-9780321503626) , Michael Feathers氏による書籍 [_Working Effectively with Legacy Code_](https://www.amazon.co.uk/Working-Effectively-Legacy-Michael-Feathers/dp/0131177052), Ash Winter氏と Rob Meaney氏による書籍 [_Team Guide to Software Testability_](http://testabilitybook.com/) と Webサイト [TestabilityQuestions.com](http://TestabilityQuestions.com/) に基づいて評価基準を作成した。    

## 評価の実行方法     

評価セッション自体は、チームのふりかえりのように感じる必要があります。 通常のふりかりとの主な違いは、チーム評価セッションではファシリテーターが議論をよりしっかりと導くことです。議論する多くの質問があり、チームが利用可能な時間内にすべての評価基準を議論することが重要です。    

評価セッションの終わりには、チームは議論に基づいて、プロセスと実践を改善するためにどのようなアクションを実行するかを決定することを促され、エンパワーメントされたと感じる必要があります。    

### 評価の実行頻度    

多くの組織では、チーム評価を**3か月ごとに** 実行すると良い結果が得られることがわかっています。      

### 評価のための準備      

1.  評価セッションのファシリテーターを見つけます。これは、チームのふりかえりに精通している、チーム外の人でなければなりません。    
2.  時間を2時間、チームにとって大きなミーティングルームを確保します。         
3.  [既製のA1 PDF（リリースを参照）](https://github.com/ConfluxDigital/software-delivery-assessment/releases)を使用するか、可能であればA1サイズで、以下の個々の評価ページ（小さなマージンを使用）を使用して、各観点の評価シートを印刷します。      
	* [Team Health - 評価シート](print/print-team-health.ja.md)
	* [Deployment - 評価シート](print/print-deployment.ja.md)
	* [Flow - 評価シート](print/print-flow.ja.md)
	* [Continuous Delivery - 評価シート](print/print-continuous-delivery.ja.md)
	* [Operability - 評価シート](print/print-operability.ja.md)
	* [Testing and Testability - 評価シート](print/print-testability.ja.md)   
4.  詳細ページをガイドとして印刷（またはページを画面上で開く）して、各評価基準のコンテキストと詳細を理解します。     
	1. [Team Health](team-health.ja.md)
	2. [Deployment](deployment.ja.md)
	3. [Flow](flow.ja.md)
	4. [Continuous Delivery](continuous-delivery.ja.md)
	5. [Operability](operability.ja.md)
	6. [Testing and Testability](testability.ja.md)
5.  マーカーまたはホワイトボードマーカーをたくさん用意してください。赤、青、緑が最適です。     
6.  セッションに**ふりかえりのファシリテーションに精通している人**（おそらくスクラムマスター）を含めます。 チームの他の人はセッション中にファシリテーターから学習し、後に他の評価セッションでファシリテートできるようになります。     

> **ファシリテーター**
> 
> ファシリテーターは、セッションを実行する前に[Spotify Squad Health Check](https://labs.spotify.com/2014/09/16/squad-health-check-model/)のアプローチに慣れる必要があります。優れたレポートとして、[How I Used the Spotify Squad Health Check Model](http://www.barryovereem.com/how-i-used-the-spotify-squad-health-check-model/)、SkyBet [Squad Health Checks](https://engineering.skybettingandgaming.com/2017/02/01/squad-health-checks/)で公開されており、SpotifyからSquad Health Checkを説明する文書([PDF](https://spotifylabscom.files.wordpress.com/2014/09/squad-health-check-model2.pdf)) がダウンロードできます。      
>
> 評価セッション中に実施すること:
> 
> *	いくつか議題が長引く場合は、セッションの外でディスカッションを行うように依頼して、セッションがスケジュール通り進むようにする。   
> * 印刷された評価シートにチームのスコアとメモを書き留める。
> * 完成した評価シートの写真を撮る。    
> * エンジニアリング評価の意義と実施結果についてチームからフィードバックを受け取る。 - 笑顔で十分。        
> 

### 時間調整      

チーム評価セッションは2時間で実行され、ファシリテーターは6つの観点の質問を通して、セッションをファシリテートします。        

1.  Team health check - **35分**
2.  Deployment health check - **10分**
3.  Flow check - **10分**
4.  Continuous Delivery check - **20分**
5.  Operability check - **20分**
6.  Test coverage check - **20分**

これら6つの評価の間に**5分の休憩**を挟みます。      

### 評価セッションの実行     

各セクションにはいくつかのルールがあります。各質問には以下の記載事項を意識して回答する必要があります。      

  - チームは、個人またはチームとして、***Tired* and *Inspired*** ガイドラインに基づいて、SAD（1 OR 2）/MEH（3）/ YAY（4 OR 5） を使用して各評価基準を評価します。    

      - *Tired* は評価が低く (1), *Inspired* は評価が高い (5) です。　　　　
    
      - 個人ごとに評価した場合は、評価を集計し、1-5の単一のチームスコアを決定します。印刷されたシートに異なる色のペンを使用して、異なる評価を視覚的に示すと便利です。    

  - 過去に評価を実施している場合は、前回のスコアに対する**トレンド** を決定します。(上がった, 変わらない, 下がった)     
  
  - 今後数カ月にわたり、評価基準のスコア改善することに**同意する**。
    
  - **メモ**欄を使用して、評価のまとめ役が知る必要があると思われる詳細情報を示す。           

  - 各シートの下部にある **日付/名前/ファシリテーター** 欄に必ず情報を記入する。       
  
  - 記入済みの各シートの写真を撮り、評価のまとめ役に送信する。     
  
  - チームメンバーに次の観点から評価セッション自体を評価してもらいます： **価値**、**実行** （悪い、まあまあ、良い）    

### ファシリテーションを促進する      

各チームの評価セッションには、ファシリテーターから学習している1人の人物が参加しているため、今後のセッションをファシリテートすることができます。新しいファシリテーターはそれぞれ、少なくとも2つの他のチームとのセッションをファシリテーションする必要があります。このようにして、ファシリテーターの数は急速に拡大し、最初のファシリテーターの負担を最小限に抑えることができます。          

## 結果の調整と解釈    

各チームが評価セッションを実行して結果を送信した後、評価のまとめ役は異なるチームの結果を照合し、組織全体で改善が必要な領域を特定する必要があります。     
改善が必要な領域を特定するには、次のような質問をします。     

* チームABCがテストカバレッジについて1と評価するのは何故ですか？ スコアの上昇を妨げているものは何ですか？    

* より多くのチームのリリースを支援するために、組織として何ができますか？     

* チームがよりよく、効率良く作業できるように、プラットフォーム側が改善するべき点はありますか？

チームを直接ランク付けまたは比較しようとしないでください。代わりに、チームからのシグナルを使用して組織のダイナミクスをより理解し、組織全体の改善に優先順位を付けます。     

