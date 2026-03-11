<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/logo_dark_mode.png">
  <source media="(prefers-color-scheme: light)" srcset="./assets/logo_light_mode.png">
  <img alt="logo" src="./assets/logo_light_mode.png">
</picture>

```js
class Philosophy {
  life() {
    return 'Life is limited. Time will not wait.';
  }

  mindset() {
    return 'Every "no" is the next opportunity — keep moving.';
  }

  growth() {
    return 'Learn daily. Improve constantly. Stay curious.';
  }

  mission() {
    return 'Build clean, useful, and meaningful things.';
  }

  purpose() {
    return 'Make life better — even in small ways.';
  }
}

export default new Philosophy();
```
