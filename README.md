## マテリアル
[GitHub for developers](http://ikeike443.github.io/training-kit/courses/github-for-developers.html)

### gitツール

[Git for Windows](https://git-for-windows.gåithub.io/)  

### git資料

[Gitチートシート](https://services.github.com/kit/downloads/ja/github-git-cheat-sheet.pdf) - PDF  
[Pro Git 2 eBook](http://git-scm.com/book/ja/v2) - Gitの一番詳しい電子書籍。無料。日本語。GitHubの共同設立者＆Gitのエヴァンジェリスト @schacon さん著

### その他

[GitHub Guides](https://guides.github.com/)  
[GitHub Training & Guides](https://www.youtube.com/watch?v=FyfwLX4HAxM&list=PLg7s6cbtAD15G8lNyoaYDuKZSKyJrgwB-) - Youtube (日本語字幕付)  
[Emoji seacher](http://emoji.muan.co/) - 絵文字検索 @muan さん

## git setup

### アカウント

nameとemailはGitHubに作ったアカウントと一致させてください。  
`$ git config --global user.name "name"`  
`$ git config --global user.email "email address"`  

確認  
`$ git config --list | grep name`  
`$ git config --list | grep email`  

### 表示と改行コードの設定

`$ git config --global color.ui auto`  

Windows  
`$ git config --global core.autocrlf true`  
Mac/Linux  
`$ git config --global core.autocrlf input`  

改行コードを変換させない場合には、
`$ git config --global core.autocrlf false`  

### Windowsユーザ

Git Bashでの日本語の文字化け対策  
`$ git config --global core.quotepath false`  
  
CommitメッセージをvimではなくNotepadで入力する場合。  
`$ git config --global core.editor notepad`  
*NotepadはデフォルトがSJISのため、日本語はWEB上で文字化けしますのでご注意ください。*
  
サクラエディタを指定してもOK。秀丸も指定できます。  
`$ git config --global core.editor "'C:/Program Files/sakura/sakura.exe' -CODE=4"`  
*sakura.exeのパスは、各自のローカルでご確認ください。*

### HTTP Proxy  

`$ git config --global http.proxy http://proxy/`  

### その他

GitHub Enterpriseを自己署名証明書で運用する場合  
`$ git config --global http.sslVerify false`
