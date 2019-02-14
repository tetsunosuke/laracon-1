# PHP テストワークショップ @ Laravel JP Conference

こちらの資料は、[Laravel JP Conference](https://conference2019.laravel.jp/)の[PHPテストワークショップ](https://fortee.jp/laravel-jp-conference-2019/proposal/f3964b26-c9db-4ee5-abee-c9b0ea51db7f)で使用するものになります。

## 概要

【はじめに】

皆さん、普段ユニットテストコードを書いていますか？  
テストは私たちが実装するプログラムが期待通りの動作をしていない場合に自動検知することができ、「間違ったコードを書かない」ために必要不可欠といえます。  
しかし、正しいテストを書くには、どの程度のテストコードを書けば必要十分かを学び、同値分析や境界値分析などの専門知識を身につける必要があり、簡単なスキルとはいえません。  
このワークショップではまずテストの基礎知識やメリット・デメリットを再確認し、その後に堅牢なWEBアプリケーションを作成するためのテストの書き方をハンズオン形式で学びます。  

【タイムスケジュール】  
13:00～13:10　概要説明  
13:10～13:40　テストのメリット・デメリットを再確認  
13:40～14:20　初めてのユニットテスト  
14:20～15:50　本格的なテストのハンズオン  
15:50～16:00　まとめ  

【注意事項】  
本ワークショップはトータル180分間（3時間）を予定します。  
参加される際には以下の注意事項をよくお読みのうえご準備ください。  

■注意事項  
座学の後にお手持ちのノートPCを使ってプログラム実装を行って頂きますので、必ずノートPCをお持ち下さい。  
また以下の準備が完了していない場合、ハンズオンを受講できない場合があります。  

1. 以下の手順に沿ってPHPがインストールされていること
http://php.net/manual/ja/install.php

2. 以下の手順に沿ってcomposerがインストールされているこ
https://getcomposer.org/download/

3. PHPプログラムを書くためのテキストエディタがインストールされていること
PHPStorm・VS Code等、普段お使いのもので結構です

■想定する受講者  
PHPプログラムをこれまでに概ね3ヶ月以上開発した事があり、基礎的な文法知識を身につけている方を対象としています。  
これまで全くPHPプログラムを開発したことがない方は対象としておらず、ハンズオンで十分なサポートができませんので、予めご了承ください。  

[PHPテストワークショップ](https://fortee.jp/laravel-jp-conference-2019/proposal/f3964b26-c9db-4ee5-abee-c9b0ea51db7f)より、抜粋

## 進め方  
以下のディレクトリ構成を参考にハンズオンを進めてください。

```
├─src
│ ├─basic（基礎問題が配置してあります）
│ └─authentic（応用問題が配置してあります）
│ 
├─tests（testソースを置く場所になります）
│ ├─basic（あなたが作成した基礎問題のテストコードを配置します）
│ │ └─WS1Test.php（←のようなファイル名でテストコードを記述してください
│ └─authentic（あなたが作成した応用問題のテストコードを配置します）
│ └─Template.php（テストで使用する基本的なコードが記述されているテンプレートになります）
│ 
├─answer（答えが配置しています。どうしてもわからないときに確認してください
│ ├─basic（基礎問題の答えです）
│ └─authentic（応用問題の答えです）
│ 
├─vendor
│ └─phpunitがインストールされる場所
├─.gitignore
├─composer.json （phpunitの依存性を記載）
├─composer.lock
└─README.md（このREADME.mdになります）
```

