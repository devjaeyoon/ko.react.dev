# 번역을 위한 모범 사례

<https://github.com/reactjs/ko.react.dev/issues/27>

## 쌍점은 거의 사용하지 않습니다

한국어 맞춤법에서는 쌍점(colon, 콜론)을 사용하는 경우를 규정하고 있는데 항목의 열거나 희곡 대사 등에서만 제한적으로 사용합니다([참고](https://korean.go.kr/kornorms/regltn/regltnView.do?regltn_code=0001&regltn_no=753#a753)). 특히 영어처럼 문장 끝에 쌍점을 붙이는 경우는 없으므로 주의하세요.

```text
👍모범 사례
다음 예시를 보세요.

👎잘못된 사례
다음 예시를 보세요:
```

## '시'는 제한적으로 사용합니다

존칭을 표현하는 '-시-'는 문장의 간결함을 해칠 수 있습니다. `~하세요`처럼 제한적인 경우에만 사용하고 그 외에는 사용하지 않는 편이 좋습니다. 다만, 작업자들끼리 대화할 때는 존중의 의미에서 사용해도 상관없습니다.

```text
👍모범 사례
살펴보면 좋습니다.

👍모범 사례
살펴보세요.

👎잘못된 사례
살펴보시면 좋습니다.
```

## 쉼표를 모두 옮길 필요는 없습니다

영어와 우리말에서 쉼표를 사용하는 사례가 다릅니다. 우리말에서 쉼표를 사용하는 몇 가지 경우는 [맞춤법](https://korean.go.kr/kornorms/regltn/regltnView.do?regltn_code=0001&regltn_no=732#a732)에 규정되어 있습니다. 꼭 필요할 때만 사용하고 그 외에는 제한하는 편이 좋을 것 같습니다.

```text
🇬🇧 For example, if `id` is the row ID, either of the following would work

👍모범 사례
예를 들어 `id`가 행의 ID일 경우 다음 코드가 모두 작동합니다.

👎잘못된 사례
예를 들어, `id`가 행의 ID일 경우 다음 코드가 모두 작동합니다.
```

## render = 렌더링하다

`render`나 `bind`처럼 우리말 번역이 없고 원문의 음만 따서 쓰는 동사는 명사형 + `~하다`로 번역하는 게 좋습니다.

```text
🇬🇧 React renders DOM elements.

👍모범 사례
React는 DOM 엘리먼트를 렌더링합니다.

👎잘못된 사례
React는 DOM 엘리먼트를 렌더합니다.

👍모범 사례
함수를 바인딩해야 합니다.
```

## '당신'과 '여러분'은 없어도 됩니다

아주 가끔 꼭 필요할 때가 있기는 하지만 영어 표현에 많은 `당신`이나 `여러분`, `우리`같은 표현은 안 쓰는 게 훨씬 자연스럽습니다.

```text
🇬🇧 Let's say you want to output "Hello, world" in a DOM element.

👍모범 사례
DOM 엘리먼트에 "Hello, World"를 표현한다고 생각해봅시다.

👎잘못된 사례
당신이 DOM 엘리먼트에 "Hello, World"를 표현하고 싶다고 생각해봅시다.
```

## 피동형 문장에 주의하세요

사실 원칙대로라면 `~되다`같은 수동태도 가능하면 억제하는 편이 좋지만 실제로 작업을 하다 보면 써야 문장이 자연스러울 때도 있습니다. 다만 `보여지다`, `생각되다`와 같은 불필요한 피동형 문장은 자제하는 편이 좋습니다.

```text
🇬🇧 Elements appeared on the screen.

👍모범 사례
화면에 보이는 엘리먼트.

👎잘못된 사례
화면에 보여지는 엘리먼트.
```

## 똑같은 표현은 비슷한 표현으로 대체하면 문장이 더 유려해집니다

번역문에서 흔히 나타나는 문제가 영어 단어를 1:1로 번역하다 보니 표현이 단조로워진다는 점입니다. 예를 들어 `common`은 `일반적으로`라고만 번역한다거나 `call`은 `호출한다`라고만 번역하는 사례가 많습니다. 가까운 위치에서 똑같은 표현이 여러 차례 등장할 때 조금씩 표현을 바꾸어주면 문장이 더 읽기 좋아집니다. `common`이나 `commonly`는 `일반적으로`, `널리`, `흔히` 등으로 바꿀 수 있고 `call`, `invoke` 등은 `호출하다`, `실행하다` 등으로 바꿀 수 있습니다.

```text
👍모범 사례
이때 흔히 사용되는 패턴은 일반 자바스크립트 객체를 전달하는 것이다.

👎잘못된 사례
이때 일반적으로 사용되는 패턴은 일반 자바스크립트 객체를 전달하는 것이다.
```

## 어색하지 않다면 단수형을 사용합시다

원래 우리말에서는 `~들`이라는 복수형 표현을 그리 널리 사용하지 않습니다. 물론 문장의 의미에 따라 반드시 복수의 객체임을 명시해야 할 때가 있긴 하지만, 그 외의 경우라면 단수형으로 표현하는 편이 대체로 자연스럽습니다.

```text
🇬🇧 The examples below demonstrate the differences.

👍모범 사례
아래 예시는 위에서 언급한 차이점을 보여줍니다.

👍모범 사례 - 복수형 표현이 필요한 경우
아래 예시는 위에서 언급한 여러 차이점을 보여줍니다.

👎잘못된 사례
아래 예시들은 위에서 언급한 차이점들을 보여줍니다.
```

## If는 생략할 수도 있습니다

`If`로 시작하는 문장의 번역이 항상 `만약`으로 시작할 필요는 없습니다. 틀린 번역은 아니지만 한국어에서는 `~한다면`이라는 어미가 이미 조건 또는 상황의 가정을 의미하므로 때로는 `만약`이 없어도 충분히 말이 됩니다. 아래 예시는 인접한 두 문장이 모두 `만약`으로 시작하고 있었습니다. 한 문장 만이라도 `만약`을 생략하면 조금 더 읽기 수월해집니다.

```text
🇬🇧If you load React from a `<script>` tag, .... If you use ES6 with npm, ...

👍모범 사례
React를 <script> 태그로 불러온다면 ... ES6와 npm을 함께 사용한다면 ...

👎잘못된 사례
만약 React를 <script> 태그로 불러온다면 ... 만약 ES6와 npm을 함께 사용한다면 ...
```
