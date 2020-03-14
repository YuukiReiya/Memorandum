URL:https://qiita.com/m-yamazaki/items/45ea4a71ebb769995043

git status = git status -unormal
と同じ。
なので、新規（＝追跡されていない）ディレクトリに含まれているファイルは表示されない！

git status -uall
とすることで表示されるようになる。

デフォルトの設定方法
【表示させる場合】
git config status.showUntrackedFiles all
【表示しない場合】
git config status.showUntrackedFiles no