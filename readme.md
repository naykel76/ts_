<p align="center"><a href="https://naykel.com.au" target="_blank"><img src="https://avatars0.githubusercontent.com/u/32632005?s=460&u=d1df6f6e0bf29668f8a4845271e9be8c9b96ed83&v=4" width="120"></a></p>


# Vite starter project with Type Script an vanilla Javascript

Run development server:

```bash
npm run dev
```

Build project:

```bash
npm run build
```

Preview build project:

```bash
npm run preview
```

## Component Example

```ts
// src/counter.ts
export function setupCounter(element: HTMLButtonElement) {
  let counter = 0
  const setCounter = (count: number) => {
    counter = count
    element.innerHTML = `count is ${counter}`
  }
  element.addEventListener('click', () => setCounter(counter + 1))
  setCounter(0)
}
```

```js
// src.main.ts
import { setupCounter } from './counter.ts'
setupCounter(document.querySelector<HTMLButtonElement>('#counter')!)
```
