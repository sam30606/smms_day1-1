## Running the app

```bash
# development
$ npm run start
```

## main.ts
```ts
async function bootstrap() {
  const app = await NestFactory.create(AppModule);
  await app.listen(4000);
}
bootstrap();
```
## app.controller.ts
```ts
  @Get("helloworld")
  getHello(): string {
    return this.appService.getHello();
  }
```

## 簡介
基本上就是跑 ```nest new smms_day1-1``` 來產生新專案

改port，改app.controller.ts的route

ngrok ```ngrok http 4000```