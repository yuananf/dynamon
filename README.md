# :smiling_imp: Dynamon. DynamoDB GUI client

![Logo](assets/dynamon.png) [![CircleCI](https://circleci.com/gh/deptno/dynamon.svg?style=shield)](https://circleci.com/gh/deptno/dynamon)

Dynamon is GUI client for DynamoDB.

---
> version 0.3 was failed to deploy use `dynamon@0.2`
## Recent update
- support Local dynamodb stream(v0.3)
![Stream](assets/dynamon-stream.gif)
- Drop {electron, monorepo} to develop fast
- Connect dynamodb-local (`docker run -p 8000:8000 amazon/dynamodb-local`)
```json
{
  "region": "dynamon",
  "endpoint": "http://localhost:8000"
}
```
- Support create table

---

> unstable (dynamon developed targeting local environment)

[![](https://user-images.githubusercontent.com/1223020/38453064-7a2d421c-3a8a-11e8-821f-c607fff85642.png)](https://www.youtube.com/watch?v=UI9xyrAKAg0&feature=youtu.be)
:eyes: Click to watch screenshot

- [Old electron version](https://github.com/deptno/dynamon/releases)

## run

```bash
npm -g i dynamon
dyanmon # run
```

## contribution

```bash
npm i
npm run watch # for backend typescript compile
npm run start
```

### Logging

```bash
DEBUG=dynamon* npm run start # dynamon only
DEBUG=dynalee* npm run start # dynalee(aws-sdk wrapper, engine for dynamon)
DEBUG=dyna* npm run start # dynamon, dynalee
DEBUG=* npm run start # ??
```

## features

* [x] Local DynamoDB (port 8000)
* View
  * Table view
    * [x] Sub collection view
    * [x] Table schema view
    * [ ] ~~Nested JSON(Enter, Leave)~~
  * [x] JSON view
* Operation
  * Table
    * [x] Add Table
    * [ ] Edit Table
    * [x] Delete Table
  * Search
    * [x] Scan
    * [ ] Query
    * [ ] Index
  * Document
    * [ ] Add multiple documents
    * [x] Add document
    * [ ] Edit document
    * [ ] Delete document
* [x] Stream - support function endpoint
    
## link
- [LICENSE](LICENSE)
- [CHANGELOG](CHANGELOG)
- [Dynalee - Heart of dynamon](https://github.com/deptno/dynalee) 
