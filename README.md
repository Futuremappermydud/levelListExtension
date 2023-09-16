# levelListExtension

![Beat Saber 2023_09_16 17_44_18](https://github.com/scifiHerb/levelListExtension/assets/109839172/aa4b49de-ee4f-496b-8cdf-e5a9a2544c1f)  
![Beat Saber 2023_09_16 17_59_56](https://github.com/scifiHerb/levelListExtension/assets/109839172/1d2f1d37-e25a-43ed-9af8-d97554cd034d)


# 説明
ビートセイバーの譜面リスト拡張MODです、指定した難易度のハイスコア(存在しない場合下の難易度）をリストに表示します.

対応バージョンはSteamVR版の1.29.1まで、β2.0からはBeatLeaderに対応しました

# 使い方
ModSettingsのlevelListExtensionからRefreshもしくは初回起動時に譜面選択画面で譜面情報を取得します  
Priorityに設定している方の譜面が優先して取得される仕様なので優先順位を変更した後は読み込み直す必要があります。   

譜面リスト上のボタンで指定した難易度、もしくはプレイリストに指定されている難易度のハイスコアを表示します。  

# ChangeLog  
2023-9-16  
・BeatLeaderに対応しました、どちらを優先して取得するか選択できます  
・Lawless、OneHandなども読み込むようにしました  

・色設定でScoreSaber取得時、BeatLeader取得時で星とppの色の設定項目追加しました。  

2023-9-6

・クリアランクの各精度、色を設定ファイルから指定できるようにしました。

・難易度表示の色を設定できるようにしました。

2023-9-4

・カスタムソングタブを選択した状態でゲームを終了した際次起動時フリーズする不具合修正しました。

・Modifierに対応しました。

・プレイリストに難易度が設定されてる場合優先して読み込む設定を付けました、プレイリストの難易度を表示している際は末尾にアスタリスクが付きます。
またModSettingsをシンプルに作り直しました。  
# 設定項目 
設定ファイル：(\Beat Saber\UserData\levelListExtension.json)

譜面データ：(\Beat Saber\UserData\levelListExtension_Songs.json)

# 不具合他
・一部譜面でScoreSaberからMaxScoreが取得できない場合があり正常に表示されないことがあります  
・同一譜面で別々の難易度が設定されている場合片方のみ表示されます  
・プレイリストの選択時のデータを使用しているので初回起動時はプレイリストを選択し直す必要があります。  

・"enable":           MODのOn Off    

・"refresh":          trueにすると起動時譜面を(count * 8)取得します、取得後自動でfalseになります。

・"priorityPlaylist": プレイリストに難易度が設定されている場合selectDiffに関わらず、プレイリストの難易度を優先して表示します、その場合リスト末尾に*が付きます。

・"selectDiff":  指定難易度（0=easy,4=expert plus)
  
・"count":        取得譜面数（一度に8譜面取得するのでcount*8譜面取得します)

・"Rank~"スコアランクの各精度、色を設定できます  
・"Difficulty~"  Difficultyの色設定です  
・"scoreSaberColor/beatLeaderColor"  星の色設定です
・"listChoice" (Score Saber / Beat Leader) 優先するデータを変更できます

