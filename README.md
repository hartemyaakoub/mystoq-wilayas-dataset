# Mystoq Wilayas Dataset

> Open dataset of Algeria's **58 wilayas** with metadata useful for any
> e-commerce or logistics app in Algeria.

## What's included

- `wilayas.json` - all 58 wilayas:
  - official code (01-58)
  - name in English, Arabic, French
  - Yalidine delivery coverage (boolean)

## Use it

```bash
curl -L https://raw.githubusercontent.com/hartemyaakoub/mystoq-wilayas-dataset/main/wilayas.json
```

```js
const wilayas = await fetch(
  "https://cdn.jsdelivr.net/gh/hartemyaakoub/mystoq-wilayas-dataset/wilayas.json"
).then(r => r.json());
```

## License

CC0 1.0 - public domain. Use it however you want, no attribution required.

## Powered by

[Mystoq](https://mystoq.com) - the simplest cash-on-delivery e-commerce
platform for Algeria. Built by [Hartem Yaakoub](https://hartem.tkawen.com).

Other open datasets and tools from us:
- [mystoq-openapi](https://github.com/hartemyaakoub/mystoq-openapi)
- [mystoq-themes](https://github.com/hartemyaakoub/mystoq-themes)
- [awesome-mystoq](https://github.com/hartemyaakoub/awesome-mystoq)
