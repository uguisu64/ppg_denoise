# ppg_denoise

## 概要

研究室で，PPGの最低限のノイズ除去に関して調査と実践を行ったので，それの結果まとめ．

参照性向上のためにGithubにあげます．

## 結果について

今回は移動平均を用いたノイズ除去と，バンドパスフィルタ的なノイズ除去について実践しました．

どちらの移動平均を用いる場合は適切な窓幅を選択することで，適切なノイズ除去が行えます．今回のデータに関しては窓幅50，データは60Hzのため，0.8s程度の窓幅であればよい結果が得られました．

バンドパスフィルタでは，基本的によい結果を得られたのではないのかなと思います．ただし，BPMが早い場合は未検証のため，要追加検証かなと思います．