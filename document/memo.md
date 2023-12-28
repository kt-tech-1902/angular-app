# memo

## 画面描写までの流れ

index.html が画面に表示される。

1. main.ts から実行される
2. app.component.ts を指定してルートコンポーネントとしてレンダリングする。(スタンドアロンコンポーネントとして)
   ```ts
   bootstrapApplication(AppComponent, {
     providers: [provideProtractorTestingSupport(), provideRouter(routeConfig)],
   }).catch((err) => console.error(err));
   ```
   - bootstrapApplication：ルートコンポーネントとしてレンダリング
   - provideProtractorTestingSupport：E2E テスト実施に使用
   - provideRouter：Routing の設定を指定
3. app.component.ts に app-root がセレクタとして定義されているため、index.html 内の<app-root>に置き換わる
4. app.component.ts に実装された内容が画面に表示される
