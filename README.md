# tkinterGUI

## 解説
新聞販売店における「組込み」作業用のアプリケーションです。
従来は帳簿で管理されていた情報をWindows端末で管理するためのものです。

## 仕様
Windows10、Windows11で起動します。
Windowsタブレットでの利用を想定したアプリケーションです。  
顧客の名称の下の色のついた横棒をクリックすると顧客情報を編集できます。

## 開発環境
python-3.7.4

## デプロイ
1⃣Window用Python環境[Winpython](https://sourceforge.net/projects/winpython/files/WinPython_3.7/3.7.4.1/)をダウンロードする。
    例としてWinpython64-3.7.4.1.exeをダウンロードする。
	
2⃣Winpython64-3.7.4.1.zipを展開し.exeファイルを実行。
	例として分かりやすいディレクトリ「C:\」を指定。
	終了するまでしばらく待つ．

3⃣システム環境変数の設定
    コントロールパネル→システム→システムの詳細設定→環境変数、を選択する。
    システム環境変数(Path)  に次を追加  
    ```
    C:\WPy64-3741\python-3.7.4.amd64
    ```  
    ```
    C:\WPy64-3741\python-3.7.4.amd64\Scripts
    ```  
    コマンドプロンプトの新しいウィンドウを開く。


4⃣パッケージのインストール
    コマンドプロンプトで下記を実行する。
    pip と python にパスが通っていることを確認する。  
    ```
    where pip
    ```  
    ```
    where python 
    ```  
    pipアップグレード。  
    ```
    python -m pip install --upgrade pip
    ```  
    次のコマンドを実行。  
    ```
    pip install pysmb
    ```  
    ```
    pip install openpyxl
    ```  
    ```
    pip install pyttsx3
    ```

5⃣アプリケーションの起動
    コマンドプロンプトで下記を実行する。  
    ```
    cd C:\gui\dawn\scripts\
    ```  
    ```
    C:\WPy64-3741\python-3.7.4.amd64\python.exe app.py
    ```  
    またはエクスプローラーでC:\gui\dawn\scriptsを開いてapp.pyをクリックする。


## 作成者
JiroScript  
E-mail:geektakedown@gmail.com

