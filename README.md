# Svelte Amplifyテストレポジトリ

問題解決能力を高めるためのレポジトリです。

```
yarn dev
で起動するようにし、
localhost:5000
でアクセスしたときにConsoleにエラーが出ないようにしてください。
```

なお、このレポジトリは、Svelteのテンプレートを落としてきて、それに対してAmplify Authのライブラリを入れただけです。

```
import { Auth } from '@aws-amplify/auth'
```

を入れるとエラーになるので、それをどうにかして解決してください。

## 成功条件
- `import { Auth } from '@aws-amplify/auth'` の記載がちゃんと実行される位置にある。(src配下のコードは変更しない）
- yarn devがエラーなく成功する（WarningのみはOK)
- yarn dev後、 http://localhost:5000 にアクセスして、Webページが表示され、DevToolsのコンソールにエラーが出ていない

## 注意事項
- Authを別のパッケージからimportするのはNGです。
- importしたAuthがundefinedでないことを確認してください。
- yarn build ではなく、 yarn dev してください。
