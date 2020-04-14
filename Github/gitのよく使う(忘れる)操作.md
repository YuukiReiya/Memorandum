//リモートを含め、全ブランチ名の取得
git remote branch -a

//リモート上のブランチを削除
git remote origin --delete ブランチ名
  もしくは
git push origin :ブランチ名

//ブランチ名の変更(変更対象上のブランチで操作)
git branch -m 変更後のブランチ名

