# levelListExtension
ビートセイバーの譜面リスト拡張MODです、指定した難易度のハイスコア(存在しない場合下の難易度）をリストに表示します.

対応バージョンは1.29.1までなのと、新ノーツを含む譜面(V3)はScoreSaberにデータがないため取得できません。

またOculus版のビートセイバーはSteam版とIDの取得方法が違うのでSteam版のみ対応となってます。

![Beat Saber 2023_08_28 16_51_44](https://github.com/scifiHerb/levelListExtension/assets/109839172/70d496e8-b7d0-46ac-87c3-9f3b6c4b60e3)


# 使い方
ModSettingsからlevelListExtensionのrefreshボタンで過去のプレイ履歴を一括取得します、取得はバックグラウンドで行うので設定から抜けても問題ありません。

難易度の指定は譜面リストの右上のボタンから順送りで指定できます。

取得数はデフォルトで800ですが設定ファイル(\Beat Saber\UserData\levelListExtension.json)のCount数から指定できます。


# 設定項目 
(\Beat Saber\UserData\levelListExtension.json)

・"Enable":      MODのOn Off

・"selectDiff":  指定難易度（0=easy,4=expert plus)
  
・"count":        取得譜面数（一度に8譜面取得するのでcount*8譜面取得します)
