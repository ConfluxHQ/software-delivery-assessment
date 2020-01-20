# Deployment check

> **Part of the Multi-team Software Delivery Assessment** ([README](README.md))
> 
> Copyright © 2018-2019 [Conflux Digital Ltd](https://confluxdigital.net/)
> 
> Licenced under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) ![CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/3.0/88x31.png)
>
> _Permalink: [SoftwareDeliveryAssessment.com](http://SoftwareDeliveryAssessment.com/)_ 

Based on the maturity questions from Mirco Hering, author of [*DevOps for the Modern Enterprise*](https://notafactoryanymore.com/2018/03/01/mircos-self-assessment-questions-of-devops-maturity/)

Mirco Hering氏のブログ投稿[_DevOps for the Modern Enterprise_](https://itrevolution.com/book/devops_modern_enterprise/) で説明されている書籍[_DevOps for the Modern Enterprise_](https://itrevolution.com/book/devops_modern_enterprise/) の主要な質問に基づいています。          

目的：*ソフトウェアのデプロイのプラクティスに対するチームの自信を評価すること*    

方法：[Spotify Squad Health Check](https://labs.spotify.com/2014/09/16/squad-health-check-model/) のアプローチを使用して、次の質問に対するチームの回答を評価する:   

| **質問**                                                                                                                                 | **しんどい (1)**                                                        | **すばらしい (5)**                                             |
| -------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------- | ------------------------------------------------------------ |
| 1\. **環境の再構築** - **環境を破壊し、保存された構成から再構築**をした場合どうなりますか？ | 何が起こるかわからない-環境は不安定だ        | 問題なし - デプロイメント・パイプラインで既にテストしている |
| 2\. **新規設定** - **アプリケーション構成を削除して再デプロイ**をした場合どうなりますか？                              | 何が起こるかわからない-設定プロセスは不安定だ | 問題なし - デプロイメント・パイプラインで既にテストしている |
| 3\. **アプリケーションの再デプロイ** - **プログラムの変更はなく、アプリケーションを再デプロイ**をした場合どうなりますか？                      | 何が起こるかわからない-デプロイは不安定だ         | 問題なし - デプロイメント・パイプラインで既にテストしている |
| 4\. **テストの再実行** - **テストスイートを再実行**した場合どうなりますか？                                            | 何が起こるかわからない-テストスイートは本当に不安定だ    | 問題なし - デプロイメント・パイプラインで既にテストしている |

