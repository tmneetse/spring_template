# spring_template

## quick start

```bash
# 設定ファイルを記述する、DBのスキーマとユーザーとパスワードを設定
cp -p .env.sample .env
vi .env

# アプリケーション側の設定、上記で設定したDBの設定を書き込む
cp -p app/src/main/resources/application.yml.sample app/src/main/resources/application.yml
vi app/src/main/resources/application.yml

# 起動
docker-compose up -d
```

## Generate code by swagger

```bash
# Ref https://github.com/int128/gradle-swagger-generator-plugin
./gradlew generateSwaggerCode
```
