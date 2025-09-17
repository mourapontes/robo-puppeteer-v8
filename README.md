# Robo de Aulas

[![Build Linux Installer](https://github.com/mourapontes/robo-puppeteer-v8/actions/workflows/build-linux-installer.yml/badge.svg)](https://github.com/mourapontes/robo-puppeteer-v8/actions/workflows/build-linux-installer.yml)
[![Release Linux (.deb)](https://github.com/mourapontes/robo-puppeteer-v8/actions/workflows/release-linux.yml/badge.svg)](https://github.com/mourapontes/robo-puppeteer-v8/actions/workflows/release-linux.yml)

Automação de preenchimento de aulas usando Electron + Puppeteer.

## Downloads

- Releases: https://github.com/mourapontes/robo-puppeteer-v8/releases
- Último artefato de CI: ver em Actions → Build Linux Installer

## Como usar (ChromeOS / Linux)

Consulte o `README_CHROMEOS.md` para instruções completas.

Resumo:
```bash
sudo apt update
sudo apt install -y libgtk-3-0 libnss3 libxss1 libasound2
# Baixe o .deb da aba Releases
sudo dpkg -i ./Robo-de-Aulas-*.deb
sudo apt --fix-broken install
```

## Desenvolvimento local

```bash
npm install
npm start
```

## Build

```bash
npm run dist
```
O instalador será gerado em `dist/`.

## Release automática

Para criar uma Release com `.deb` anexado:
```bash
git tag -a v1.0.1 -m "Release v1.0.1"
git push origin v1.0.1
```

---
Feito com ❤️ para facilitar seu fluxo de trabalho.
