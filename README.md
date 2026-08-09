<!--
  - SPDX-FileCopyrightText: 2026 G2W Tecnologia
  - SPDX-FileCopyrightText: 2017 Nextcloud GmbH and Nextcloud contributors
  - SPDX-License-Identifier: GPL-2.0-or-later
-->
# G2W Cloud — Cliente Desktop

**Seus arquivos. Sua nuvem. Sem limites.**

Fork do [Nextcloud Desktop Client](https://github.com/nextcloud/desktop) (tag `v34.0.1`, versão estável — não a `master`/dev) com a marca da **G2W Tecnologia** — sincroniza arquivos do [G2W Cloud](https://github.com/gabrielpst/g2wcloud) com seu computador, Windows/macOS/Linux.

## O que é

Cliente de sincronização de pasta pro **G2W Cloud** (nosso servidor próprio, fork do Nextcloud). Mesma função do cliente oficial do Nextcloud — sincronização em segundo plano, seleção de pastas, arquivos virtuais — só que com a marca e as URLs de suporte da G2W em vez da Nextcloud GmbH.

## Por que uma tag estável, e não a `master`

O `nextcloud/desktop` upstream mantém a `master` como branch de **desenvolvimento** (hoje em `34.1.0 alpha`). Este fork parte da tag **`v34.0.1`**, a última versão lançada.

## Marca

Toda a identidade (nome, ícones, cores do assistente de configuração, URLs de atualização/ajuda) fica centralizada em [`NEXTCLOUD.cmake`](NEXTCLOUD.cmake) — mecanismo oficial de white-label do projeto, sem precisar tocar em código-fonte. Ícones em [`theme/colored/`](theme/colored/).

## Instalação / Build

Requer Qt 6, CMake e as dependências padrão do projeto Nextcloud Desktop — ver [`doc/`](doc/) e [`CONTRIBUTING.md`](CONTRIBUTING.md) upstream (o processo de build é idêntico ao original, só a marca muda).

## Manter atualizado

Este fork acompanha os lançamentos da `v34.x` upstream:

```bash
git remote add upstream https://github.com/nextcloud/desktop.git
git fetch upstream --tags
git merge v34.0.X   # trocar pela tag mais recente
```

## Licença

[GPL-2.0-or-later](COPYING), a mesma do projeto original. Ver [`LICENSES/`](LICENSES/) para as licenças de cada dependência.

## Contato

**G2W Tecnologia**
Site: [cloud.g2wtecnologia.net](https://cloud.g2wtecnologia.net/)
WhatsApp: +55 67 99608-6281
E-mail: contato@g2wtecnologia.net
