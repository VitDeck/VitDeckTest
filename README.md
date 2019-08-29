# VitDeckについて
VitDeckは多人数で特定のルールに沿ったUnityのアセットを同時に制作するプロジェクトを支援するツールです。
以下の機能を持っています。
- 管理者が事前に準備したテンプレート（フォルダ構成やシーンファイル）から提出用アセットの作成を開始する
- 制作物が管理者が構成したルールに沿っているかチェックする
- 提出用のUnitypackageを作成する
- テンプレートやルールのアップデート用unitypackageを配布する

作業管理者がVitDeckをフォークし、テンプレートおよびチェック用のルールを構成した上で作業者に配布することを前提にしています。

# ツール構成方法
VitDeckの各機能の構成方法は以下を参照してください。
- [テンプレートの作成方法](https://github.com/vkettools/VitDeck/wiki/MakingTemplate)
- [ルールセットの作成方法](https://github.com/vkettools/VitDeck/wiki/MakingRuleSet)
- [エクスポート設定の作成方法](https://github.com/vkettools/VitDeck/wiki/MakingExportSetting)
- [アップデート通知の構成](https://github.com/vkettools/VitDeck/wiki/ConfiguringUpdateNortification)

# 検証可能なルール
VitDeckでは検証したいルールの組み合わせとその設定をルールセットと呼ばれる単位で管理します。
管理者は最初に[ルールセットを構成](https://github.com/vkettools/VitDeck/wiki/MakingRuleSet)してください。
以下のルールが最初から利用でき、独自ルールも定義可能です。
- 指定のUnityバージョンで動作しているか検証
- アセット名の使用禁止文字の検出
- 特定のGUIDを持つアセットの検出
- アセットの長すぎるパスの検出
- 特定の拡張子を持つアセットの検出
- ブースがBounds内に収まっているかの検証
- コンポーネントのホワイトリスト検証
- コンポーネントのブラックリスト検証
- エラーシェーダーの検出
- Noneになっているメッシュの検出
- missingになっている参照の検出

# 動作環境
以下の環境でテストしています。
- Windows 10
- Unity 2017.4.28f1

# License
Copyright (c) 2019 VitDeck

Released under the MIT license.
