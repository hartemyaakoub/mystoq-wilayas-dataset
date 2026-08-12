# Mystoq Wilayas Dataset

Open dataset of Algeria's **69 wilayas**, in Arabic and Latin script.

> **Updated for the 2026 administrative reform.** Algeria now has 69 wilayas, not 58.
> Eleven were promoted from délégations to full wilayas (codes 59–69: Aflou, Barika,
> Ksar Chellala, Messaad, Ain Oussara, Ras El Oued, Ain Beida, Bou Saâda,
> El Abiodh Sidi Cheikh, and others). Datasets still listing 58 are out of date.

## What's included

`wilayas.json` — all 69 wilayas:

- `code` — official code, `01`–`69`
- `name_ar` — name in Arabic
- `name` — name in Latin script

```json
{"code":"16","name_ar":"الجزائر","name":"Alger"}
```

## Use it

```bash
curl -L https://raw.githubusercontent.com/hartemyaakoub/mystoq-wilayas-dataset/main/wilayas.json
```

```js
const wilayas = await fetch(
  "https://cdn.jsdelivr.net/gh/hartemyaakoub/mystoq-wilayas-dataset/wilayas.json"
).then(r => r.json());
```

## What is deliberately not here

A `yalidine` coverage flag used to sit on each row. It has been removed rather than
carried forward: there is no verified coverage data for the eleven new wilayas, and a
dataset that guesses is worse than one that omits. Ask your carrier for current
coverage — it changes.

Commune-level data is not in this file. Earlier descriptions mentioned communes; the
dataset has only ever contained wilayas.

## Source

Generated from the wilaya table the [Mystoq](https://mystoq.com) platform reads on
every order, so it matches what a live Algerian cash-on-delivery checkout actually uses.

## License

CC0 1.0 — public domain. Use it however you want, no attribution required.

---

Built by [Hartem Yaakoub](https://github.com/hartemyaakoub) · part of the TKAWEN ecosystem.
