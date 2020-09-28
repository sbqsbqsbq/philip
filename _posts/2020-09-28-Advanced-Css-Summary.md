---
title: "Advanced CSS and Sass 강의 내용 정리 9월 28일자"
date: 2020-09-28 11:24:28 -0400
categories: Summary
---

Jonas Schmedtmann의 Advanced Css and Sass: Flexbox, Grid, Animations and More! 강의를 들으면서, 생각나는 점 및 내용을 정리하는 포스트이다.

sass내부에서 `[class^=something]`은 something으로 시작하는 모든 class attribute를 선택하는 selector이다.
또한, `[class$=something]`은 something으로 끝나는 모든 class attribute를 선택하는 selector이며, `[class*=something]`은 something을 포함하는 모든 class attribute를 선택하는 selector라고 할 수 있다.

Grid를 나눌 때 사용되는 1차적인 레이아웃은 Float이다. Float이후에는 Flexbox, Grid 등의 레이아웃이 사용되는데, 이번 Natour 프로젝트에서는 Float 레이아웃으로 먼저 프로젝트를 끝마치고, 차후 프로젝트에서 Flexbox와 Grid 등을 차례대로 도입할 것이다.
