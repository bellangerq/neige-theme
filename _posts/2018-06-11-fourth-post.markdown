---
title: Fourth post
date: 2018-06-11 13:17:00 Z
layout: post
---

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent egestas, nibh quis laoreet aliquam, metus quam bibendum enim, sed auctor quam odio a mi. Sed semper nisi sed diam maximus elementum. In condimentum porttitor rutrum. In viverra placerat tincidunt. Aliquam eget molestie neque. Quisque placerat risus ac urna aliquam, placerat consequat dui iaculis. Phasellus sodales leo nec diam eleifend, ut venenatis mauris pulvinar. Aliquam vel purus lacus. Suspendisse mattis aliquet arcu, laoreet rutrum ex aliquam non.


```css
.class {
  color: #ff0000; /* Cool red */
  font-size: 32px;
}
```

```javascript
const pluckDeep = key => obj => key.split('.').reduce((accum, key) => accum[key], obj)

const compose = (...fns) => res => fns.reduce((accum, next) => next(accum), res)

const unfold = (f, seed) => {
  const go = (f, seed, acc) => {
    const res = f(seed)
    return res ? go(f, res[1], acc.concat([res[0]])) : acc
  }
  return go(f, seed, [])
}
```

```html
<div class="posts">
  <article>
    <h2><a href="#">My awesome title</a></h2>
    <p>Lorem ipsum...</p>
  </article>
</div>
```
