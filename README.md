# Órbita — Prospecção de clientes para sites

Aplicativo em português para encontrar negócios locais sem site cadastrado no OpenStreetMap, qualificar oportunidades e acompanhar a prospecção.

## Publicar no GitHub Pages

1. Abra **Settings → Pages** neste repositório.
2. Em **Build and deployment**, selecione **Deploy from a branch**.
3. Escolha a branch `main`, pasta `/(root)` e clique em **Save**.
4. O site ficará em `https://andersonx553-beep.github.io/Sorteio.fut/`.

## Chave Geoapify

No aplicativo, abra **Ajustes → Chave Geoapify** e salve sua chave. Ela fica no armazenamento local deste navegador; o código público e este repositório não contêm sua chave. A versão GitHub Pages consulta a Geoapify direto do navegador. Restrinja a chave no Geoapify MyProjects usando o domínio `andersonx553-beep.github.io` como origem/referrer permitida e habilite CORS para os serviços necessários. A Geoapify permite restringir chaves por origem e HTTP referrer: https://apidocs.geoapify.com/docs/places/

Os leads também ficam neste navegador. Exporte um backup antes de trocar de dispositivo. “Sem site” significa sem site registrado no OpenStreetMap, não confirmação de que a empresa não tenha site fora da base.

## Código-fonte

O pacote `Orbita-v2-source.zip` contém o projeto fonte, incluindo a versão Cloudflare e o adaptador estático usado para compilar este GitHub Pages. Para recriar o site, extraia o pacote, instale com `pnpm install --frozen-lockfile` e rode `pnpm run build:pages`.
