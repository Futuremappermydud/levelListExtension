# levelListExtension
ビートセイバーの譜面リスト拡張MODです、指定した難易度のハイスコア(存在しない場合下の難易度）をリストに表示します.

対応バージョンはSteamVR版の1.29.1まで、新ノーツを含む譜面(V3)はScoreSaberにデータがないため取得できません。

![Beat Saber 2023_08_29 20_02_03](https://github.com/scifiHerb/levelListExtension/assets/109839172/1b92b31a-7a6a-4b2c-bb47-90a7a34d9bff)

# 使い方
初回起動時譜面の読み込みを行います、再読み込みはコンフィグファイルのReshreshをTrueにすることで可能です。
譜面リスト上のボタンで指定した難易度のハイスコアを表示します。


# 設定項目 
(\Beat Saber\UserData\levelListExtension.json)

・"Enable":      MODのOn Off

・"selectDiff":  指定難易度（0=easy,4=expert plus)
  
・"count":        取得譜面数（一度に8譜面取得するのでcount*8譜面取得します)

・"Refresh":      起動時譜面を(count * 8)取得します。
