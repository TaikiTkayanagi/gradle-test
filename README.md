# コマンド
* プロジェクトの生成
`gradle init --type java-library`
* タスク結果のみ表示する
`gradle -q {task名}`
* パラメータを渡す
`gradle {task名} -P{プロパティ名=値}`

# 注意点
* lib内に、build.gradleがある場合、`./gradlew {タスク名}`で実行する

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

# 基本タスク
* compileJava:コンパイルする
* processResources:リソースファイルをクラスのディレクトリ内にコピーする
* classes:ソースコードのコンパイルとリソースファイルのコピーを行う
* test:プログラムのテストを行う
* jar:プログラムをコンパイルし、リソースファイルなどを準備した後、それらをJarファイルにパッケージ化する
* javadoc:ソースコードを解析してJavadocファイルを生成する
* clean:ビルドにより生成されたファイルをすべて消去する

# 補足
* パスに日本語が入っていると`gradle java`は失敗する
