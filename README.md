# [Waktaverse Games](https://waktaverse.games) GameSDK (Node.js) &middot; [![Apache 2.0 License](https://img.shields.io/badge/license-Apache2.0-blue.svg)](./LICENSE) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](.github/CONTRIBUTING.md)

이 라이브러리는 [Waktaverse Games](https://waktaverse.games)에서 제공하는 API를 쉽게 이용할 수 있는 TypeScript/JavaScript GameSDK Client이에요.<br />

## 설치하기

```sh
$ npm install --save @wakgames/gamesdk
```

## SDK 사용법

### 기본 사용법

> WakGames 클래스를 불러와 사용하면 됩니다.

```ts
import {WakGames} from '@wakgames/gamesdk';

const wakGames = new WakGames({
  clientId: 'isol_dia',
  redirectUrl: 'https://example.com/callback',
});
```

### 초기화

> Serialize Field를 필수로 설정해야 합니다.

- clientId : 개발자 포탈에서 확인된 Client ID.
- redirectUrl : 개발자 포탈에서 설정한 Callback URL.

### API

> 모든 API는 Promise를 반환합니다. (Async)<br>
> Promise 인자는 결과 데이터와 상태 코드로 구성된 RestAPI Response 객체입니다.<br>
> (단, Authorize API는 창을 열어야 할 URL을 담은 object를 반환합니다.)

> API 호출이 실패한 경우 Fetch Exception이 발생합니다.<br>
> 상세한 설명은 JSDoc을 참고해주세요.

## 기여하기

이 라이브러리는 누구나 기여할 수 있어요. 라이브러리에 기여하고 싶다면 아래 문서를 참고해주세요. [(기여 가이드라인)](./.github/CONTRIBUTING.md)

## 라이선스

MIT License. [LICENSE](./LICENSE) 파일을 참고하세요.<br />
본 레포지토리를 상업적 용도로 Fork/재배포 하는 행위를 금합니다.
