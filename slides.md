---
# You can also start simply with 'default'
theme: dracula
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: 이동윤, 자기소개
info: |
  ## 자기소개 시작 하나 둘 셋!

  Learn more at [Sli.dev](https://sli.dev)
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
class: text-center
fonts:
  mono: "Noto Sans Mono"
  sans: "Nanum Pen Script"
  serif: "Nanum Pen Script"
---

<style>
@font-face {
  font-family: 'Nanum Pen Script';
  src: url('/assets/fonts/NanumPenScript-Regular.ttf') format('truetype');
  font-weight: normal;
  font-style: normal;
}

body {
  font-family: 'Nanum Pen Script', 'Arial', sans-serif;
}

h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}

</style>

  <!-- 상단 (고정 높이) -->
  <div class="absolute top-0 text-2xl inset-x-0 p-2 color-white">
    <span>안녕하세요 저는</span>
  </div>
  
  <!-- 중앙 (유연한 확장) -->
  <div class="flex-1 p-4">
    <p class="text-9xl">이동윤입니다.</p>
  </div>
  
  <!-- 하단 (고정 높이) -->

  <div @click="$slidev.nav.next" class="absolute border border-white rounded bottom-4 w-xl  left-50 p-2" hover:bg="white op-10"> 만나서 반갑습니다! 😆 
  </div>
  <div class="absolute border border-white rounded text-xl bottom-4 right-0 border-white ">
    <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="slidev-icon-btn">
      <carbon:edit />
    </button>
    <a href="https://github.com/SpookyJelly/introduce-self" target="_blank" class="slidev-icon-btn">
      <carbon:logo-github />
    </a>
  </div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
level: 2
---

# 조작법

좌하단에 호버되는 컨트롤 패널 혹은 아래의 키보드 단축키를 이용해보세요😆😆

|                                                    |                             |
| -------------------------------------------------- | --------------------------- |
| <kbd>right</kbd> / <kbd>space</kbd>                | 다음 애니메이션 혹은 슬라이드로     |
| <kbd>left</kbd> / <kbd>shift</kbd><kbd>space</kbd> | 이전 애니메이션 혹은 슬라이드로|
| <kbd>up</kbd>                                      | 이전 슬라이드로             |
| <kbd>down</kbd>                                    | 다음 슬라이드로                 

---

# Who am I?

<span v-mark.underline.orange>
  간결한 코드로 안정적으로 동작하는 프로그램을 좋아하는 3년차 프론트엔드 개발자입니다.
</span>

<br>
<br>
또한 저는...
<br>
<br>

- 🛠 **UX 엔지니어** - 기술과 디자인의 교차점에서 사용자 중심 솔루션을 고민합니다.
- 🧑‍💻 **테크 얼리 어뎁터** - 새로운 기술에 대해 관심이 많으며, 프론트엔드 생태계가 어떻게 변하고 있는지 주목합니다.
- 🤹 **오픈소스 컨트리뷰터** - 오픈소스에 기여하는 것을 좋아하며, 다양한 사람과 의견을 나눕니다.
  <br>
  <br>

이기도 하고요!

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/features/slide-scope-style
-->


<!--
Here is another comment.
-->
---
layout: two-cols
---


# TMI!


<div class='text-2xl'>
  <ol>
    <li class='m-8'>MBTI: <span v-mark.circle.orange='1'> ENTJ </span> </li>
    <li class='m-8'>취미 : <span v-mark.circle.orange='2'>운동, 게임</span></li>
    <li class='m-8'>최애 치킨 : 
   <span v-mark.circle.orange='3'>KFC 오리지널</span> 
    </li>
  </ol>
</div>

<arrow v-if="$slidev.nav.clicks === 1" x1="120" y1="450" x2="175" y2="170" color="#953" width="2" arrowSize="1" />

<arrow v-if="$slidev.nav.clicks === 2" x1="120" y1="450" x2="175" y2="250" color="#953" width="2" arrowSize="1" />

<arrow v-if="$slidev.nav.clicks === 3" x1="120" y1="450" x2="175" y2="310" color="#953" width="2" arrowSize="1" />

<div class='absolute bottom-5 p-5 border border-white rounded' v-if="$slidev.nav.clicks === 1">
근데 저 아무리 봐도 J가 아니라 P인거 같아요. 그래서 그냥 엔팁으로 살려고요.
</div>

<div class='absolute bottom-5 p-5 border border-white rounded' v-if="$slidev.nav.clicks === 2">
운동 (웨이트 트레이닝)은 매일 꾸준히 하고 있고, 게임은 AAA급 게임, 인디게임 가리지 않고 즐깁니다. 같이 하고 싶으신분 (운동이든 게임이든)은 편하게 말해주세요!
</div>

<div class='absolute bottom-5 p-5 border border-white rounded' v-if="$slidev.nav.clicks === 3">
치킨의 왕은 KFC이며, 오리지널 치킨은 그 정통한 계승자이다. 반박은 받지 않습니다.
</div>


::right::

<div class="relative">
  <!-- 첫 번째 이미지 -->
  <img v-if="$slidev.nav.clicks === 1"
  src="/assets/images/mbti.jpg" alt="Image 1" class="image-container" />

  <!-- 두 번째 이미지 -->
  <img v-if="$slidev.nav.clicks === 2" src="/assets/images/steam.png" alt="Image 2" class="image-container" />

  <!-- 세 번째 이미지 -->
  <img v-if="$slidev.nav.clicks === 3" src="/assets/images/favor.png" alt="Image 3" class="image-container" />
</div>

<style>

.image-container{
  width: 100%;
  height: 58vh;
  object-fit: contain;
  border-radius: 8px;
}

  
</style>
---

# 저는 이런 기술을 가지고 있습니다!



````md magic-move {lines: true}
```ts {1,3-8}
// 이런 언어들을 주로 다루고
export default {
  language(){
    return [
      "typescript",
      "python"
    ]
  }
}
```


```ts {1,3-9}
// 이런 라이브러리들를 좋아하며,
export default {
  libs(){
    return [
      "react",
      "storybook",
      "visx",
      "ramda.js"
    ]
  }
}
```

```ts {1,3-10}
// 이런 기술들에 관심이 많습니다!
export default {
  tools(){
    return [
      "docker",
      "WebGL",
      "AWS",
      "Neovim"
    ]
  }
}
```



````

---

# 오픈소스 활동들
##### 제 오픈소스 활동들을 소개합니다.

<br/>
<v-switch>
  <template #0>
    <div>
      <strong>sb-addon-permutation-table</strong>
      <div class="flex gap-8">
        <div class="image-layout">
          <img class="image-container" src="/assets/images/demo-sb.gif" />
        </div>
        <div class="flex flex-col basis-1/2">
          <div class="flex grow">
          <ul>
            <li>컴포넌트의 형상들을 하나의 스토리에서 볼 수 있게 해주는 storybook 애드온</li>
            <li>Storybook community addon 선정</li>
          </ul>
          </div>
          <div class="border-t border-white">
            <a href="https://www.npmjs.com/package/sb-addon-permutation-table" target="_blank" class="slidev-icon-btn">
              <carbon:logo-npm />
            </a>
            <a href="https://daimresearch.github.io/sb-addon-permutation-table/?path=/docs/introduction--docs" target="_blank" class="slidev-icon-btn">
              <carbon:demo />
            </a>
          </div>
        </div>
      </div>
    </div>
  </template>

  <template #1>
    <div>
      <strong>cheesy-stories</strong>
      <div class="flex gap-8">
        <div class="image-layout">
          <img class="image-container" src="/assets/images/demo-chessy.gif" />
        </div>
        <div class="flex flex-col basis-1/2">
          <div class="flex grow">
          <ul>
            <li>Story의 width를 인터렉티브하게 조절할 수 있는 stroybook 애드온</li>
            <li>width change에 따라 변경되는 형상을 빠르게 확인 가능</li>
          </ul>
          </div>
          <div class='border-t border-white'>
            <a href="https://github.com/SpookyJelly/cheesy-stories" target="_blank" class="slidev-icon-btn">
              <carbon:logo-npm />
            </a>
            <a href="https://spookyjelly.github.io/cheesy-stories/" target="_blank" class="slidev-icon-btn">
              <carbon:demo />
            </a>
          </div>
        </div>
      </div>
    </div>
  </template>

  <template #2>
    <div>
      <strong>applejelly</strong>
      <div class="flex gap-8">
        <div class="image-layout">
          <img class="image-container" src="/assets/images/demo-aj.png" />
        </div>
        <div class="flex flex-col basis-1/2">
          <div class="flex grow">
          <ul>
            <li>Datadog의 DRUIDS에 영감을 받은 컴포넌트 라이브러리</li>
            <li>🔥Now in progress🔥</li>
          </ul>
          </div>
          <div class='border-t border-white'>
            <a href="https://www.npmjs.com/package/applejelly" target="_blank" class="slidev-icon-btn">
              <carbon:logo-npm />
            </a>
            <a href="https://spookyjelly.github.io/applejelly/?path=/docs/introduction--docs" target="_blank" class="slidev-icon-btn">
              <carbon:demo />
            </a>
          </div>
        </div>
      </div>
    </div>
  </template>
</v-switch>


<style>

.image-container{
  width: 100%;
  height: 30vh;
  object-fit: contain;
  border-radius: 8px;
}
.image-layout{
  width:50%;
}

  
</style>
---
## class: px-20
---

# 포트로직스에서 이루고 싶은 것들



### 물류 디지털화 기여
  직관적이고 효율적인 프론트엔드 UI를 개발해 포트로직스의 물류 시스템 사용자 경험을 개선하고, 디지털 전환에 기여하고 싶습니다.



### 코드 품질 향상
  Storybook과 Swagger를 활용해 코드 문서화와 API 형상 관리를 체계화하여, 팀의 개발 효율성과 유지보수성을 높이고 싶습니다.



### 기술 심화
  React와 TypeScript를 심화 학습하며, 포트로직스의 프론트엔드 솔루션을 안정적이고 확장 가능하게 발전시키고 싶습니다.



### 협업과 상생
  데이터 기반 논거로 타 팀과 협업해 문제 해결 중심의 개발 문화를 만들어, 동료와 고객에게 인정받는 성과를 내고 싶습니다.

---
layout: statement
---

# 읽어주셔서 감사합니다!!

### 앞으로 잘 부탁드리겠습니다!

## 이동윤, Frontend Dev of Portlogics


<br/>
<div>
 <carbon:mobile/> 010-8326-2964
 <div />
 <carbon:email/> yoon@portlogics.com
</div>
