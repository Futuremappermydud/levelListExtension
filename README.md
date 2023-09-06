# levelListExtension

2023-9-6

・クリアランクの各精度、色を設定ファイルから指定できるようにしました。

・難易度表示の色を設定できるようにしました。

2023-9-4

・カスタムソングタブを選択した状態でゲームを終了した際次起動時フリーズする不具合修正しました。

・Modifierに対応しました。



(β1.3)
試験的にプレイリストに難易度が設定されてる場合優先して読み込む設定を付けました、プレイリストの難易度を表示している際は末尾にアスタリスクが付きます。
またModSettingsをシンプルに作り直しました。

既知の問題として
・同一譜面で別々の難易度が設定されている場合片方のみ表示されます
・プレイリストの選択時のデータを使用しているので初回起動時はプレイリストを選択し直す必要があります。

# 説明
ビートセイバーの譜面リスト拡張MODです、指定した難易度のハイスコア(存在しない場合下の難易度）をリストに表示します.

対応バージョンはSteamVR版の1.29.1まで、新ノーツを含む譜面(V3)はScoreSaberにデータがないため取得できません。

![Beat Saber 2023_09_06 16_09_51](https://github.com/scifiHerb/levelListExtension/assets/109839172/6babbe1e-ad3e-41c8-8ba3-9f0adb61b1aa)

# 使い方
初回起動時譜面の読み込みを行います、再読み込みはModSettingsのrefreshをTrueにします。
譜面リスト上のボタンで指定した難易度、もしくはプレイリストに指定されている難易度のハイスコアを表示します。

# 設定項目 
設定ファイル：(\Beat Saber\UserData\levelListExtension.json)

譜面データ：(\Beat Saber\UserData\levelListExtension_Songs.json)



・"enable":           MODのOn Off    

・"refresh":          trueにすると起動時譜面を(count * 8)取得します、取得後自動でfalseになります。

・"priorityPlaylist": プレイリストに難易度が設定されている場合selectDiffに関わらず、プレイリストの難易度を優先して表示します、その場合リスト末尾に*が付きます。

・"selectDiff":  指定難易度（0=easy,4=expert plus)
  
・"count":        取得譜面数（一度に8譜面取得するのでcount*8譜面取得します)

・"Rank~"スコアランクの各精度、色を設定できます
・"Difficulty~"  Difficultyの色設定です
