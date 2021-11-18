# コマンド
* プロジェクトの生成
`gradle init --type java-library`
* タスク結果のみ表示する
`gradle -q {task名}`
* パラメータを渡す
`gradle {task名} -P{プロパティ名=値}`

# DSLとは
* Domain Specific LAnguageの略
* 特定の用途に限定された言語を示す
* ベースとなる言語からアレンジされたもの

# プロジェクトの構成
* .gradleフォルダー
  * タスクで生成されたファイルなどが保存される
* gradleフォルダー
  * デフォルトでは、Gradle環境をまとめたラッパーファイルというファイルう類がある
* srcフォルダー
  * ソースコード関連のファイル
* build.gradle
  * Gradleのビルドファイル,ここにプロジェクトのビルド内容をGroovyで記述する
* gradlew, gradlew.bat
  * Gradleのコマンドファイル
* setting.gradle
  * 設定情報を記述したファイル
  * ビルドする前に読み込まれる、必要なライブラリーなどを記述する

# 補足
* パスに日本語が入っていると`gradle java`は失敗する
