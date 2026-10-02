# Nova iOS

Projeto do aplicativo Nova para iOS usando Capacitor.

## Estrutura

- `www/index.html` — interface e lógica atual do Nova.
- `package.json` — dependências do Capacitor.
- `capacitor.config.json` — nome e identificador do aplicativo.
- `codemagic.yaml` — workflow para gerar o projeto iOS e o IPA no Codemagic.

## Build

O workflow instala as dependências, cria a plataforma iOS com Swift Package Manager, sincroniza os arquivos web, aplica a configuração de assinatura disponível no Codemagic e executa o build do IPA.

O `codemagic.yaml` precisa permanecer na raiz do repositório.

A geração de um IPA assinado depende das credenciais de assinatura Apple configuradas no Codemagic.
