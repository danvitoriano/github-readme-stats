<div align="center">
  <img src="https://res.cloudinary.com/anuraghazra/image/upload/v1594908242/logo_ccswme.svg" width="100px" alt="GitHub Readme Stats" />
  <h1 style="font-size: 28px; margin: 10px 0;">GitHub Readme Stats</h1>
  <p>Estatísticas do GitHub geradas dinamicamente para o seu README!</p>
</div>

<p align="center">
  <a href="https://github.com/danvitoriano/github-readme-stats/actions">
    <img alt="Testes passando" src="https://github.com/danvitoriano/github-readme-stats/workflows/Test/badge.svg" />
  </a>
  <a href="https://github.com/danvitoriano/github-readme-stats/graphs/contributors">
    <img alt="Contribuidores no GitHub" src="https://img.shields.io/github/contributors/danvitoriano/github-readme-stats" />
  </a>
  <a href="https://codecov.io/gh/danvitoriano/github-readme-stats">
    <img alt="Cobertura de testes" src="https://codecov.io/gh/danvitoriano/github-readme-stats/branch/main/graph/badge.svg" />
  </a>
  <a href="https://github.com/danvitoriano/github-readme-stats/issues">
    <img alt="Issues" src="https://img.shields.io/github/issues/danvitoriano/github-readme-stats?color=0088ff" />
  </a>
  <a href="https://github.com/danvitoriano/github-readme-stats/pulls">
    <img alt="Pull requests no GitHub" src="https://img.shields.io/github/issues-pr/danvitoriano/github-readme-stats?color=0088ff" />
  </a>
  <a href="https://securityscorecards.dev/viewer/?uri=github.com/danvitoriano/github-readme-stats">
    <img alt="OpenSSF Scorecard" src="https://api.securityscorecards.dev/projects/github.com/danvitoriano/github-readme-stats/badge" />
  </a>
  <br />
  <br />
  <a href="https://vercel.com?utm\_source=github\_readme\_stats\_team\&utm\_campaign=oss">
    <img src="./powered-by-vercel.svg"/>
  </a>
</p>

> [!TIP]
> **API em produção (este fork):** `https://github-readme-stats-rouge-phi-60.vercel.app` — exemplo de cartão de estatísticas: [`/api?username=danvitoriano&show_icons=true`](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&show_icons=true). Projeto original: [anuraghazra/github-readme-stats](https://github.com/anuraghazra/github-readme-stats).

<p align="center">
  <a href="#all-demos">Ver demos</a>
  ·
  <a href="https://github.com/anuraghazra/github-readme-stats/issues/new?assignees=&labels=bug&projects=&template=bug_report.yml">Reportar bug</a>
  ·
  <a href="https://github.com/anuraghazra/github-readme-stats/issues/new?assignees=&labels=enhancement&projects=&template=feature_request.yml">Sugerir recurso</a>
  ·
  <a href="https://github.com/anuraghazra/github-readme-stats/discussions/1770">FAQ</a>
  ·
  <a href="https://github.com/anuraghazra/github-readme-stats/discussions/new?category=q-a">Fazer uma pergunta</a>
</p>


<p align="center">Curte o projeto? Considere <a href="https://www.paypal.me/anuraghazra">fazer uma doação</a> para ajudar no desenvolvimento!</p>

<details>
<summary>Índice (clique para expandir)</summary>

- [Cartão de estatísticas do GitHub](#github-stats-card)
    - [Ocultar estatísticas individuais](#hiding-individual-stats)
    - [Mostrar estatísticas extras](#showing-additional-individual-stats)
    - [Mostrar ícones](#showing-icons)
    - [Commits em um ano específico](#showing-commits-count-for-specified-year)
    - [Temas](#themes)
    - [Personalização](#customization)
- [Pins extras de repositório](#github-extra-pins)
    - [Uso](#usage)
    - [Opções](#options)
    - [Demo](#demo)
- [Pins de Gist](#github-gist-pins)
    - [Uso](#usage-1)
    - [Opções](#options-1)
    - [Demo](#demo-1)
- [Cartão de linguagens mais usadas](#top-languages-card)
    - [Uso](#usage-2)
    - [Opções](#options-2)
    - [Algoritmo das linguagens](#language-stats-algorithm)
    - [Excluir repositórios](#exclude-individual-repositories)
    - [Ocultar linguagens](#hide-individual-languages)
    - [Mostrar mais linguagens](#show-more-languages)
    - [Layout compacto](#compact-language-card-layout)
    - [Layout donut](#donut-chart-language-card-layout)
    - [Layout donut vertical](#donut-vertical-chart-language-card-layout)
    - [Layout pizza](#pie-chart-language-card-layout)
    - [Ocultar barras de progresso](#hide-progress-bars)
    - [Formato das estatísticas de linguagens](#change-format-of-languages-stats)
    - [Demo](#demo-2)
- [Cartão de estatísticas WakaTime](#wakatime-stats-card)
    - [Opções](#options-3)
    - [Demo](#demo-3)
- [Todas as demos](#all-demos)
  - [Dica rápida (alinhar cartões)](#quick-tip-align-the-cards)
    - [Estatísticas e linguagens](#stats-and-top-languages-cards)
    - [Fixar repositórios](#pinning-repositories)
- [Hospedar você mesmo](#deploy-on-your-own)
  - [GitHub Actions (recomendado)](#github-actions-recommended)
  - [Self-hosted (Vercel/outro) (recomendado)](#self-hosted-vercelother-recommended)
    - [Passo 1: obter um PAT do GitHub](#first-step-get-your-personal-access-token-pat)
    - [Na Vercel](#on-vercel)
    - [:film\_projector: Tutorial em vídeo passo a passo (@codeSTACKr)](#film_projector-check-out-step-by-step-video-tutorial-by-codestackr)
    - [Em outras plataformas](#on-other-platforms)
    - [Variáveis de ambiente disponíveis](#available-environment-variables)
  - [Manter o fork atualizado](#keep-your-fork-up-to-date)
- [:sparkling\_heart: Apoie o projeto original](#sparkling_heart-support-the-project)
</details>

<h1 id="important-notices">Avisos importantes <!-- omit in toc --></h1>

> [!IMPORTANT]
> Os exemplos neste README usam o **deploy deste fork** em `https://github-readme-stats-rouge-phi-60.vercel.app`. A instância pública original em [`github-readme-stats.vercel.app`](https://github-readme-stats.vercel.app/api) é “melhor esforço” e pode falhar por limites de taxa (veja [#1471](https://github.com/anuraghazra/github-readme-stats/issues/1471)). Usamos cache quando aplicável (veja [opções comuns](#common-options)); em produção você pode seguir com este deploy, [hospedar você mesmo](#deploy-on-your-own) ou usar [GitHub Actions](#github-actions-recommended) para SVGs estáticos no [repositório de perfil](https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme).

<img alt="Badge de disponibilidade" src="https://img.shields.io/endpoint?url=https%3A%2F%2Fgithub-readme-stats-git-monitoring-github-readme-stats-team.vercel.app%2Fapi%2Fstatus%2Fup%3Ftype%3Dshields">

> [!IMPORTANT]
> A equipe do projeto original é pequena e prioriza com base em votos :+1:. Eles usam o painel Top Issues para demanda da comunidade (veja [#1935](https://github.com/anuraghazra/github-readme-stats/issues/1935)). Vote nas issues e PRs que lhe interessam; o mais votado tende a ser atendido primeiro.

<h2 id="github-stats-card">Cartão de estatísticas do GitHub</h2>

Copie e cole no seu Markdown — pronto.

Altere o valor de `?username=` para o seu usuário do GitHub.

```md
[![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano)](https://github.com/danvitoriano/github-readme-stats)
```

> [!WARNING]
> Por padrão, o cartão mostra apenas estatísticas de repositórios públicos (estrelas, commits, PRs etc.). Para incluir dados de repositórios privados, [implante sua própria instância](#deploy-on-your-own) com um token da API do GitHub.

> [!NOTE]
> As patentes disponíveis são S (top 1%), A+ (12,5%), A (25%), A- (37,5%), B+ (50%), B (62,5%), B- (75%), C+ (87,5%) e C (todos). O esquema segue o [sistema de notas acadêmicas japonês](https://wikipedia.org/wiki/Academic_grading_in_Japan). O percentil global é uma soma ponderada dos percentis de cada métrica (commits, PRs, reviews, issues, estrelas e seguidores), com base nas CDFs [exponencial](https://wikipedia.org/wiki/exponential_distribution) e [log-normal](https://wikipedia.org/wiki/Log-normal_distribution). A implementação está em [src/calculateRank.js](https://github.com/anuraghazra/github-readme-stats/blob/master/src/calculateRank.js). O anel ao redor da patente indica 100 menos o percentil global.

<h3 id="hiding-individual-stats">Ocultar estatísticas individuais</h3>

Use o parâmetro de consulta `&hide=` com valores separados por vírgula.

> Opções: `&hide=stars,commits,prs,issues,contribs`

```md
![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&hide=contribs,prs)
```

<h3 id="showing-additional-individual-stats">Mostrar estatísticas extras</h3>

Use `&show=` com valores separados por vírgula.

> Opções: `&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage`

```md
![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage)
```

<h3 id="showing-icons">Mostrar ícones</h3>

Para exibir ícones, passe `&show_icons=true` na URL:

```md
![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&show_icons=true)
```

<h3 id="showing-commits-count-for-specified-year">Commits em um ano específico</h3>

Informe o ano com `&commits_year=YYYY` para contar só commits daquele ano.

```md
![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&commits_year=2020)
```

<h3 id="themes">Temas</h3>

Com os temas embutidos você altera a aparência sem [personalização manual](#customization).

Use `&theme=NOME_DO_TEMA`, por exemplo:

```md
![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&show_icons=true&theme=radical)
```

#### Temas embutidos

O GitHub Readme Stats inclui vários temas (ex.: `dark`, `radical`, `merko`, `gruvbox`, `tokyonight`, `onedark`, `cobalt`, `synthwave`, `highcontrast`, `dracula`).

<img src="https://res.cloudinary.com/anuraghazra/image/upload/v1595174536/grs-themes_l4ynja.png" alt="Temas do GitHub Readme Stats" width="600px"/>

Veja prévias de [todos os temas](themes/README.md) ou o [arquivo de configuração](themes/index.js). Novos temas estão em pausa para reduzir manutenção; PRs só com tema novo serão fechados.

#### Tema responsivo ao modo claro/escuro

[![Dan Vitoriano's GitHub stats-Dark](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&show_icons=true\&theme=dark#gh-dark-mode-only)](https://github.com/danvitoriano/github-readme-stats#responsive-card-theme#gh-dark-mode-only)
[![Dan Vitoriano's GitHub stats-Light](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&show_icons=true\&theme=default#gh-light-mode-only)](https://github.com/danvitoriano/github-readme-stats#responsive-card-theme#gh-light-mode-only)

Como o GitHub reenvia as imagens pela [CDN](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-anonymized-urls), o servidor não sabe o tema do usuário. Ainda assim, há quatro formas de adaptar o cartão no cliente.

##### Tema transparente

O tema `transparent` tem fundo transparente e funciona bem nos temas claro e escuro padrão do GitHub. Ative com `&theme=transparent`:

```md
![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&show_icons=true&theme=transparent)
```

<details>
<summary>:eyes: Ver exemplo</summary>

![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&show_icons=true\&theme=transparent)

</details>

##### Canal alfa transparente no `bg_color`

Use `bg_color` para deixar qualquer [tema](themes/README.md) com fundo transparente (`bg_color=00000000`):

```md
![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&show_icons=true&bg_color=00000000)
```

<details>
<summary>:eyes: Ver exemplo</summary>

![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&show_icons=true\&bg_color=00000000)

</details>

##### Tags de contexto de tema do GitHub

Use as [tags de contexto de tema](https://github.blog/changelog/2021-11-24-specify-theme-context-for-images-in-markdown/) do GitHub: acrescente `#gh-dark-mode-only` ou `#gh-light-mode-only` ao final da URL da imagem para mostrá-la só no tema escuro ou claro:

```md
[![Dan Vitoriano's GitHub stats-Dark](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&show_icons=true&theme=dark#gh-dark-mode-only)](https://github.com/danvitoriano/github-readme-stats#gh-dark-mode-only)
[![Dan Vitoriano's GitHub stats-Light](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&show_icons=true&theme=default#gh-light-mode-only)](https://github.com/danvitoriano/github-readme-stats#gh-light-mode-only)
```

<details>
<summary>:eyes: Ver exemplo</summary>

[![Dan Vitoriano's GitHub stats-Dark](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&show_icons=true\&theme=dark#gh-dark-mode-only)](https://github.com/danvitoriano/github-readme-stats#gh-dark-mode-only)
[![Dan Vitoriano's GitHub stats-Light](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&show_icons=true\&theme=default#gh-light-mode-only)](https://github.com/danvitoriano/github-readme-stats#gh-light-mode-only)

</details>

##### Recurso de mídia com `<picture>`

Com [mídia condicional](https://github.blog/changelog/2022-05-19-specify-theme-context-for-images-in-markdown-beta/) em HTML, use `<picture>` e `prefers-color-scheme` para alternar imagens por tema:

```html
<picture>
  <source
    srcset="https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&show_icons=true&theme=dark"
    media="(prefers-color-scheme: dark)"
  />
  <source
    srcset="https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&show_icons=true"
    media="(prefers-color-scheme: light), (prefers-color-scheme: no-preference)"
  />
  <img src="https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&show_icons=true" />
</picture>
```

<details>
<summary>:eyes: Ver exemplo</summary>

<picture>
  <source
    srcset="https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&show_icons=true&theme=dark"
    media="(prefers-color-scheme: dark)"
  />
  <source
    srcset="https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&show_icons=true"
    media="(prefers-color-scheme: light), (prefers-color-scheme: no-preference)"
  />
  <img src="https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano&show_icons=true" />
</picture>

</details>

<h3 id="customization">Personalização</h3>

Personalize todos os cartões com parâmetros na URL.

<h4 id="common-options">Opções comuns</h4>

| Nome | Descrição | Tipo | Valor padrão |
| --- | --- | --- | --- |
| `title_color` | Cor do título do cartão. | string (hex) | `2f80ed` |
| `text_color` | Cor do texto. | string (hex) | `434d58` |
| `icon_color` | Cor dos ícones, quando houver. | string (hex) | `4c71f2` |
| `border_color` | Cor da borda. Ignorado se `hide_border` estiver ativo. | string (hex) | `e4e2e2` |
| `bg_color` | Cor de fundo (hex ou gradiente *ângulo,cor1,cor2,...*). | string | `fffefe` |
| `hide_border` | Oculta a borda do cartão. | boolean | `false` |
| `theme` | Nome do tema; veja [temas disponíveis](themes/README.md). | enum | `default` |
| `cache_seconds` | Cache HTTP manual (mín.: 21600, máx.: 86400). | inteiro | `21600` |
| `locale` | Idioma do cartão; lista [abaixo](#available-locales). | enum | `en` |
| `border_radius` | Arredondamento dos cantos. | número | `4.5` |

> [!WARNING]
> Usamos cache para aliviar os servidores (veja <https://github.com/anuraghazra/github-readme-stats/issues/1471#issuecomment-1271551425>). Padrões: cartão de stats — 24 h; linguagens — 144 h (6 dias); pin — 240 h (10 dias); gist — 48 h; WakaTime — 24 h. Para atualizar com mais frequência, [implante sua instância](#deploy-on-your-own) e defina a [variável de ambiente](#available-environment-variables) `CACHE_SECONDS`.

##### Gradiente em `bg_color`

Vários valores separados por vírgula:

    &bg_color=GRAU,COR1,COR2,COR3...COR10

<h5 id="available-locales">Idiomas disponíveis</h5>

Lista de `locale` suportados:

<table>
<tr><td>

| Código | Idioma |
| --- | --- |
| `ar` | Arabic |
| `az` | Azerbaijani |
| `bn` | Bengali |
| `bg` | Bulgarian |
| `my` | Burmese |
| `ca` | Catalan |
| `cn` | Chinese |
| `zh-tw` | Chinese (Taiwan) |
| `cs` | Czech |
| `nl` | Dutch |
| `en` | English |
| `fil` | Filipino |
| `fi` | Finnish |
| `fr` | French |
| `de` | German |
| `el` | Greek |

</td><td>

| Código | Idioma |
| --- | --- |
| `he` | Hebrew |
| `hi` | Hindi |
| `hu` | Hungarian |
| `id` | Indonesian |
| `it` | Italian |
| `ja` | Japanese |
| `kr` | Korean |
| `ml` | Malayalam |
| `np` | Nepali |
| `no` | Norwegian |
| `fa` | Persian (Farsi) |
| `pl` | Polish |
| `pt-br` | Portuguese (Brazil) |
| `pt-pt` | Portuguese (Portugal) |
| `ro` | Romanian |

</td><td>

| Código | Idioma |
| --- | --- |
| `ru` | Russian |
| `sa` | Sanskrit |
| `sr` | Serbian (Cyrillic) |
| `sr-latn` | Serbian (Latin) |
| `sk` | Slovak |
| `es` | Spanish |
| `sw` | Swahili |
| `se` | Swedish |
| `ta` | Tamil |
| `th` | Thai |
| `tr` | Turkish |
| `uk-ua` | Ukrainian |
| `ur` | Urdu |
| `uz` | Uzbek |
| `vi` | Vietnamese |

</td></tr>
</table>

Se faltar o seu idioma, contribua! Veja [CONTRIBUTING.md — traduções](CONTRIBUTING.md#translations-contribution).

#### Opções exclusivas do cartão de estatísticas

| Nome | Descrição | Tipo | Valor padrão |
| --- | --- | --- | --- |
| `hide` | Oculta [itens indicados](#hiding-individual-stats). | string (lista separada por vírgula) | `null` |
| `hide_title` | Oculta o título do cartão. | boolean | `false` |
| `card_width` | Largura manual do cartão. | número | `500px (aprox.)` |
| `hide_rank` | Oculta a patente e ajusta a largura. | boolean | `false` |
| `rank_icon` | Ícone alternativo da patente: `github`, `percentile` ou `default`. | enum | `default` |
| `show_icons` | Ícones ao lado das métricas. | boolean | `false` |
| `include_all_commits` | Conta todos os commits, não só o ano atual. | boolean | `false` |
| `line_height` | Altura da linha entre textos. | inteiro | `25` |
| `exclude_repo` | Exclui repositórios. | string (lista) | `null` |
| `custom_title` | Título personalizado. | string | `<username> GitHub Stats` |
| `text_bold` | Texto em negrito. | boolean | `true` |
| `disable_animations` | Desliga animações. | boolean | `false` |
| `ring_color` | Cor do anel da patente. | string (hex) | `2f80ed` |
| `number_format` | Formato numérico: `short` (ex.: `6.6k`) ou `long` (ex.: `6626`). | enum | `short` |
| `number_precision` | Casas decimais no formato `short` (0 a 2); ignorado em `long`. | inteiro (0, 1 ou 2) | `null` |
| `show` | Mostra [métricas extras](#showing-additional-individual-stats) (`reviews`, `discussions_started`, etc.). | string (lista) | `null` |
| `commits_year` | Só commits do ano indicado. | inteiro _(AAAA)_ | `<ano atual> (até a data)` |

> [!WARNING]
> Títulos customizados devem estar [codificados na URL](https://en.wikipedia.org/wiki/Percent-encoding) (ex.: `Estatísticas do João` → `Estat%C3%ADsticas%20do%20Jo%C3%A3o`). Use [urlencoder.org](https://www.urlencoder.org/) se preferir.

> [!NOTE]
> Com `hide_rank=true`, a largura mínima é 270 px + título e padding.

***

<h2 id="github-extra-pins">Pins extras de repositório</h2>

Permite “fixar” mais de 6 repositórios no perfil via README.

Você não fica limitado aos 6 pins nativos do GitHub.

<h3 id="usage">Uso</h3>

Copie o código abaixo e ajuste os links.

Endpoint: `api/pin?username=danvitoriano&repo=github-readme-stats`

```md
[![Readme Card](https://github-readme-stats-rouge-phi-60.vercel.app/api/pin/?username=danvitoriano&repo=github-readme-stats)](https://github.com/danvitoriano/github-readme-stats)
```

<h3 id="options">Opções</h3>

Use as [opções comuns](#common-options) e as exclusivas da tabela.

| Nome | Descrição | Tipo | Padrão |
| --- | --- | --- | --- |
| `show_owner` | Mostra o nome do dono do repositório. | boolean | `false` |
| `description_lines_count` | Número de linhas da descrição (1–3). Se omitido, ajusta automaticamente. | número | `null` |

<h3 id="demo">Demo</h3>

![Readme Card](https://github-readme-stats-rouge-phi-60.vercel.app/api/pin/?username=danvitoriano\&repo=github-readme-stats)

Com `show_owner` o nome do dono aparece no cartão:

![Readme Card](https://github-readme-stats-rouge-phi-60.vercel.app/api/pin/?username=danvitoriano\&repo=github-readme-stats\&show_owner=true)

<h2 id="github-gist-pins">Pins de Gist</h2>

Exibe Gists fixados no perfil via README.

<h3 id="usage-1">Uso</h3>

Copie o código e ajuste os links.

Endpoint: `api/gist?id=bbfce31e0217a3689c8d961a356cb10d`

```md
[![Gist Card](https://github-readme-stats-rouge-phi-60.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d)](https://gist.github.com/Yizack/bbfce31e0217a3689c8d961a356cb10d/)
```

<h3 id="options-1">Opções</h3>

[Opções comuns](#common-options) + tabela abaixo.

| Nome | Descrição | Tipo | Padrão |
| --- | --- | --- | --- |
| `show_owner` | Mostra o dono do Gist. | boolean | `false` |

<h3 id="demo-1">Demo</h3>

![Gist Card](https://github-readme-stats-rouge-phi-60.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d)

Com `show_owner`:

![Gist Card](https://github-readme-stats-rouge-phi-60.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d\&show_owner=true)

<h2 id="top-languages-card">Cartão de linguagens mais usadas</h2>

Mostra as linguagens mais presentes no código do usuário no GitHub.

> [!WARNING]
> Por padrão, só entram repositórios públicos. Para privados, [implante sua instância](#deploy-on-your-own) com token.

> [!NOTE]
> “Top languages” não mede habilidade; é uma métrica de volume de código no GitHub. É um recurso do github-readme-stats.

> [!WARNING]
> Considera só repositórios próprios **não-fork**; não inclui contribuições em repos de outras pessoas ou organizações (limitação da API). Para evoluir isso, apoie [esta discussão](https://github.com/orgs/community/discussions/18230) ([@rickstaa](https://github.com/rickstaa)).

> [!WARNING]
> Hoje só os **primeiros 100 repositórios** entram na conta, por limite da API e estabilidade das instâncias públicas ([#1471](https://github.com/anuraghazra/github-readme-stats/issues/1471)). No futuro isso pode melhorar com Action ou variáveis de ambiente.

<h3 id="usage-2">Uso</h3>

Copie e ajuste os links.

Endpoint: `api/top-langs?username=danvitoriano`

```md
[![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano)](https://github.com/danvitoriano/github-readme-stats)
```

<h3 id="options-2">Opções</h3>

[Opções comuns](#common-options) + tabela abaixo.

| Nome | Descrição | Tipo | Padrão |
| --- | --- | --- | --- |
| `hide` | Oculta [linguagens](#hide-individual-languages). | string (lista) | `null` |
| `hide_title` | Oculta o título. | boolean | `false` |
| `layout` | Layout: `normal`, `compact`, `donut`, `donut-vertical` ou `pie`. | enum | `normal` |
| `card_width` | Largura manual. | número | `300` |
| `langs_count` | Quantidade de linguagens (1–20). | inteiro | `5` em `normal`/`donut`, `6` nos demais |
| `exclude_repo` | Exclui repositórios. | string (lista) | `null` |
| `custom_title` | Título personalizado. | string | `Most Used Languages` |
| `disable_animations` | Desliga animações. | boolean | `false` |
| `hide_progress` | Esconde percentuais e barras (layout compacto). | boolean | `false` |
| `size_weight` | Peso no algoritmo ([detalhes](#language-stats-algorithm)). | inteiro | `1` |
| `count_weight` | Peso no algoritmo ([detalhes](#language-stats-algorithm)). | inteiro | `0` |
| `stats_format` | `percentages` ou `bytes`. | enum | `percentages` |

> [!WARNING]
> Nomes de linguagens e título customizado devem estar na URL codificados ([percent-encoding](https://en.wikipedia.org/wiki/Percent-encoding): `c++` → `c%2B%2B`, etc.). Use [urlencoder.org](https://www.urlencoder.org/).

<h3 id="language-stats-algorithm">Algoritmo das linguagens</h3>

Percentuais calculados assim:

```js
ranking_index = (byte_count ^ size_weight) * (repo_count ^ count_weight)
```

Por padrão só entram **bytes** (`size_weight=1`, `count_weight=0`). Ajuste com `&size_weight=` e `&count_weight=` (números reais positivos). [Mais detalhes](https://github.com/anuraghazra/github-readme-stats/issues/1600#issuecomment-1046056305).

*   `&size_weight=1&count_weight=0` — *(padrão)* ordena por bytes.
*   `&size_weight=0.5&count_weight=0.5` — *(recomendado)* mistura bytes e quantidade de repos.
*   `&size_weight=0&count_weight=1` — ordena por número de repositórios.

```md
![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano&size_weight=0.5&count_weight=0.5)
```

<h3 id="exclude-individual-repositories">Excluir repositórios</h3>

Use `&exclude_repo=repo1,repo2`.

```md
![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano&exclude_repo=github-readme-stats,danvitoriano.github.io)
```

<h3 id="hide-individual-languages">Ocultar linguagens</h3>

Use `&hide=linguagem1,linguagem2`.

```md
![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano&hide=javascript,html)
```

<h3 id="show-more-languages">Mostrar mais linguagens</h3>

`&langs_count=` aceita inteiros de 1 a 20. Padrão: `5` em `normal`/`donut` e `6` nos outros layouts.

```md
![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano&langs_count=8)
```

<h3 id="compact-language-card-layout">Layout compacto</h3>

`&layout=compact`:

```md
![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano&layout=compact)
```

<h3 id="donut-chart-language-card-layout">Layout donut</h3>

`&layout=donut`:

```md
[![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano&layout=donut)](https://github.com/danvitoriano/github-readme-stats)
```

<h3 id="donut-vertical-chart-language-card-layout">Layout donut vertical</h3>

`&layout=donut-vertical`:

```md
[![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano&layout=donut-vertical)](https://github.com/danvitoriano/github-readme-stats)
```

<h3 id="pie-chart-language-card-layout">Layout pizza</h3>

`&layout=pie`:

```md
[![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano&layout=pie)](https://github.com/danvitoriano/github-readme-stats)
```

<h3 id="hide-progress-bars">Ocultar barras de progresso</h3>

`&hide_progress=true` remove percentuais e barras (layout vira `compact`).

```md
![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano&hide_progress=true)
```

<h3 id="change-format-of-languages-stats">Formato das estatísticas</h3>

`&stats_format=bytes` mostra bytes em vez de percentual.

```md
![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano&stats_format=bytes)
```


<h3 id="demo-2">Demo</h3>

![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano)

*   Layout compacto

![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano\&layout=compact)

*   Layout donut

[![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano\&layout=donut)](https://github.com/danvitoriano/github-readme-stats)

*   Layout donut vertical

[![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano\&layout=donut-vertical)](https://github.com/danvitoriano/github-readme-stats)

*   Layout pizza

[![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano\&layout=pie)](https://github.com/danvitoriano/github-readme-stats)

*   Barras ocultas

![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano\&hide_progress=true)


*   Bytes em vez de percentual

![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano\&stats_format=bytes)

<h2 id="wakatime-stats-card">Cartão de estatísticas WakaTime</h2>

> [!WARNING]
> Só exibimos dados de perfis WakaTime **públicos**. Ative **ao mesmo tempo** “Display code time publicly” e “Display languages, editors, os, categories publicly”.

> [!WARNING]
> Contas novas podem levar até **24 horas** para aparecer no cartão.

Altere `?username=` para o seu usuário no [WakaTime](https://wakatime.com).

```md
[![Harlok's WakaTime stats](https://github-readme-stats-rouge-phi-60.vercel.app/api/wakatime?username=ffflabs)](https://github.com/danvitoriano/github-readme-stats)
```

<h3 id="options-3">Opções</h3>

[Opções comuns](#common-options) + tabela.

| Nome | Descrição | Tipo | Padrão |
| --- | --- | --- | --- |
| `hide` | Oculta linguagens listadas. | string (lista) | `null` |
| `hide_title` | Oculta o título. | boolean | `false` |
| `card_width` | Largura manual. | número | `495` |
| `line_height` | Altura da linha. | inteiro | `25` |
| `hide_progress` | Oculta barra e percentual. | boolean | `false` |
| `custom_title` | Título personalizado. | string | `WakaTime Stats` |
| `layout` | `default` ou `compact`. | enum | `default` |
| `langs_count` | Limite de linguagens; padrão = todas. | inteiro | `null` |
| `api_domain` | Domínio da API (ex.: [Hakatime](https://github.com/mujx/hakatime), [Wakapi](https://github.com/muety/wakapi)). | string | `wakatime.com` |
| `display_format` | `time` (tempo) ou `percent` (percentuais). | enum | `time` |
| `disable_animations` | Desliga animações. | boolean | `false` |

> [!WARNING]
> Título customizado na URL deve estar [codificado](https://en.wikipedia.org/wiki/Percent-encoding) (`WakaTime%20Stats`). Use [urlencoder.org](https://www.urlencoder.org/).

<h3 id="demo-3">Demo</h3>

![Harlok's WakaTime stats](https://github-readme-stats-rouge-phi-60.vercel.app/api/wakatime?username=ffflabs)

![Harlok's WakaTime stats](https://github-readme-stats-rouge-phi-60.vercel.app/api/wakatime?username=ffflabs\&hide_progress=true)

*   Layout compacto

![Harlok's WakaTime stats](https://github-readme-stats-rouge-phi-60.vercel.app/api/wakatime?username=ffflabs\&layout=compact)

***

<h2 id="all-demos">Todas as demos</h2>

*   Padrão

![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano)

*   Ocultando métricas

![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&hide=contribs,issues)

*   Métricas adicionais

![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&show_icons=true\&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage)

*   Com ícones

![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&hide=issues\&show_icons=true)

*   Logo do GitHub no lugar da patente

![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&rank_icon=github)

*   Percentil em vez da letra da patente

![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&rank_icon=percentile)

*   Cor da borda

![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&border_color=2e4058)

*   Todos os commits

![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&include_all_commits=true)

*   Temas

Escolha entre os [temas padrão](#themes)

![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&show_icons=true\&theme=radical)

*   Gradiente

![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano\&bg_color=30,e96443,904e95\&title_color=fff\&text_color=fff)

*   Cartão de stats personalizado

![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api/?username=danvitoriano\&show_icons=true\&title_color=fff\&icon_color=79ff97\&text_color=9f9f9f\&bg_color=151515)

*   Idioma do cartão (`locale`)

![Dan Vitoriano's GitHub stats](https://github-readme-stats-rouge-phi-60.vercel.app/api/?username=danvitoriano\&locale=es)

*   Cartão de repositório

![Customized Card](https://github-readme-stats-rouge-phi-60.vercel.app/api/pin?username=danvitoriano\&repo=github-readme-stats\&title_color=fff\&icon_color=f9f9f9\&text_color=9f9f9f\&bg_color=151515)

*   Cartão de Gist

![Gist Card](https://github-readme-stats-rouge-phi-60.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d)

*   Gist com tema

![Gist Card](https://github-readme-stats-rouge-phi-60.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d&theme=calm)

*   Linguagens mais usadas

![Top Langs](https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs/?username=danvitoriano)

*   WakaTime

![Harlok's WakaTime stats](https://github-readme-stats-rouge-phi-60.vercel.app/api/wakatime?username=ffflabs)

***

<h2 id="quick-tip-align-the-cards">Dica rápida (alinhar os cartões)</h2>

Por padrão o GitHub não coloca os cartões lado a lado. Você pode usar:

<h3 id="stats-and-top-languages-cards">Estatísticas e linguagens</h3>

```html
<a href="https://github.com/danvitoriano/github-readme-stats">
  <img height=200 align="center" src="https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano" />
</a>
<a href="https://github.com/danvitoriano">
  <img height=200 align="center" src="https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs?username=danvitoriano&layout=compact&langs_count=8&card_width=320" />
</a>
```

<details>
<summary>:eyes: Ver exemplo</summary>

<a href="https://github.com/danvitoriano/github-readme-stats">
  <img height=200 align="center" src="https://github-readme-stats-rouge-phi-60.vercel.app/api?username=danvitoriano" />
</a>
<a href="https://github.com/danvitoriano">
  <img height=200 align="center" src="https://github-readme-stats-rouge-phi-60.vercel.app/api/top-langs?username=danvitoriano&layout=compact&langs_count=8&card_width=320" />
</a>

</details>

<h3 id="pinning-repositories">Fixar repositórios</h3>

```html
<a href="https://github.com/danvitoriano/github-readme-stats">
  <img align="center" src="https://github-readme-stats-rouge-phi-60.vercel.app/api/pin/?username=danvitoriano&repo=github-readme-stats" />
</a>
<a href="https://github.com/anuraghazra/convoychat">
  <img align="center" src="https://github-readme-stats-rouge-phi-60.vercel.app/api/pin/?username=anuraghazra&repo=convoychat" />
</a>
```

<details>
<summary>:eyes: Ver exemplo</summary>

<a href="https://github.com/danvitoriano/github-readme-stats">
  <img align="center" src="https://github-readme-stats-rouge-phi-60.vercel.app/api/pin/?username=danvitoriano&repo=github-readme-stats" />
</a>
<a href="https://github.com/anuraghazra/convoychat">
  <img align="center" src="https://github-readme-stats-rouge-phi-60.vercel.app/api/pin/?username=anuraghazra&repo=convoychat" />
</a>

</details>

<h2 id="deploy-on-your-own">Hospedar você mesmo (recomendado)</h2>

Como o endpoint público [não é confiável](#important-notices), recomendamos implantar com GitHub Actions ou sua própria instância. GitHub Actions é o caminho mais simples (SVGs estáticos no repositório, atualizações menos frequentes); self-host exige mais trabalho e pode servir dados mais recentes (com cache).

<h2 id="github-actions-recommended">GitHub Actions</h2>

O workflow gera SVGs estáticos e evita uma chamada à API por visualização. Por padrão usa `GITHUB_TOKEN` (só dados públicos); para estatísticas privadas, configure um [PAT](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens) como secret e passe para a action.

Crie `/.github/workflows/grs.yml` no repositório de perfil (`USUARIO/USUARIO`):

```yaml
name: Atualizar cartões do README

on:
  schedule:
    - cron: "0 3 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4

      - name: Gerar cartão de estatísticas
        uses: readme-tools/github-readme-stats-action@v1
        with:
          card: stats
          options: username=${{ github.repository_owner }}&show_icons=true
          path: profile/stats.svg
          token: ${{ secrets.GITHUB_TOKEN }}

      - name: Commitar cartões
        run: |
          git config user.name "github-actions"
          git config user.email "github-actions@users.noreply.github.com"
          git add profile/*.svg
          git commit -m "Atualizar cartões do README" || exit 0
          git push
```

Depois incorpore no README do perfil:

```md
![Stats](./profile/stats.svg)
```

Mais opções na [documentação da action](https://github.com/readme-tools/github-readme-stats-action#readme).

<h2 id="self-hosted-vercelother-recommended">Self-hosted (Vercel / outro)</h2>

Sua própria instância evita limites públicos da API e dá controle sobre cache, tokens e dados privados.

<h3 id="first-step-get-your-personal-access-token-pat">Passo 1: Personal Access Token (PAT) do GitHub</h3>

Para implantar o GitHub Readme Stats você precisa de um PAT. Abaixo: como criar e quais escopos marcar (token classic e fine-grained).

Escolha os escopos certos se quiser mostrar contribuições privadas nos cartões.

#### Token classic

* Acesse [Conta → Configurações → Developer settings → Personal access tokens → Tokens (classic)](https://github.com/settings/tokens).
* `Generate new token → Generate new token (classic)`.
* Escopos:
  * `repo`
  * `read:user`
* Gere e copie o token.

#### Token fine-grained

> [!WARNING]\
> Reduz o escopo (ex.: issues nos seus repositórios) e costuma incluir só commits públicos.

* Acesse [Fine-grained tokens](https://github.com/settings/tokens).
* `Generate new token`.
* Defina expiração.
* `All repositories`.
* Em **Repository permissions**:
  * Commit statuses: read-only
  * Contents: read-only
  * Issues: read-only
  * Metadata: read-only
  * Pull requests: read-only
* Gere e copie o token.

<h3 id="on-vercel">Na Vercel</h3>

<h4 id="film_projector-check-out-step-by-step-video-tutorial-by-codestackr">:film_projector: <a href="https://youtu.be/n6d4KHSKqGk?t=107">Tutorial em vídeo passo a passo (@codeSTACKr)</a></h4>

A API do GitHub permite cerca de 5 mil requisições/hora; a URL pública `https://github-readme-stats-rouge-phi-60.vercel.app/api` pode esbarrar nisso. Na sua Vercel, com seu token, o problema some. Use o botão Deploy abaixo.

> [!NOTE]
> Desde [#58](https://github.com/anuraghazra/github-readme-stats/pull/58), dá para lidar com mais de 5k req/h e menos downtime :grin:.

> [!NOTE]
> No plano [Pro](https://vercel.com/pricing) da Vercel, dá para subir o [maxDuration](https://vercel.com/docs/concepts/projects/project-configuration#value-definition) do [vercel.json](https://github.com/anuraghazra/github-readme-stats/blob/master/vercel.json) se os cartões estourarem tempo. Mantenha abaixo de `30` s para não estourar memória.

[![Deploy to Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/danvitoriano/github-readme-stats)

<details>
 <summary><b>:hammer_and_wrench: Passo a passo: Vercel</b></summary>

1.  Acesse [vercel.com](https://vercel.com/).
2.  `Log in`.
    ![](https://files.catbox.moe/pcxk33.png)
3.  Entre com GitHub (`Continue with GitHub`).
    ![](https://files.catbox.moe/b9oxey.png)
4.  Autorize o acesso aos repositórios, se pedido.
5.  Faça fork deste repositório.
6.  Abra o [dashboard da Vercel](https://vercel.com/dashboard).
7.  `Add New...` → `Project`.
    ![](https://files.catbox.moe/3n76fh.png)
8.  `Continue with GitHub`, busque o repositório e `Import` (ou importe repo de terceiros pelo link no rodapé).
    ![](https://files.catbox.moe/mg5p04.png)
9.  Crie um PAT conforme a [seção anterior](#first-step-get-your-personal-access-token-pat).
10. Adicione o PAT como variável de ambiente `PAT_1` (veja imagem).
    ![](https://files.catbox.moe/0yclio.png)
11. Deploy. Use o domínio gerado na URL da API.

</details>

<h3 id="on-other-platforms">Em outras plataformas</h3>

> [!WARNING]
> Uso com Express fora da Vercel **não é oficial**; existe para casos em que a Vercel não serve (ex.: [#2341](https://github.com/anuraghazra/github-readme-stats/discussions/2341)). Suporte limitado.

<details>
<summary><b>:hammer_and_wrench: Deploy em outras plataformas</b></summary>

1.  Fork ou clone conforme necessário.
2.  Mova `express` de `devDependencies` para `dependencies` no `package.json`
    <https://github.com/anuraghazra/github-readme-stats/blob/ba7c2f8b55eac8452e479c8bd38b044d204d0424/package.json#L54-L61>
3.  `npm i` se precisar.
4.  `node express.js` para subir, ou defina o entrypoint `express.js` no serviço gerenciado
    <https://github.com/anuraghazra/github-readme-stats/blob/ba7c2f8b55eac8452e479c8bd38b044d204d0424/package.json#L11>
5.  Pronto 🎉
    </details>

<h3 id="available-environment-variables">Variáveis de ambiente</h3>

Variáveis úteis para personalizar sua instância self-hosted:

<table>
  <thead>
    <tr>
      <th>Nome</th>
      <th>Descrição</th>
      <th>Valores</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>CACHE_SECONDS</code></td>
      <td>Duração do cache dos cartões em segundos. Sobrescreve os padrões da instância pública. Se não definida, o padrão costuma ser 24 h (86.400 s) onde aplicável.</td>
      <td>Inteiro positivo ou <code>0</code> para desligar cache</td>
    </tr>
    <tr>
      <td><code>WHITELIST</code></td>
      <td>Lista separada por vírgula de usuários do GitHub autorizados. Se vazia, todos podem usar.</td>
      <td>Usernames separados por vírgula</td>
    </tr>
    <tr>
      <td><code>GIST_WHITELIST</code></td>
      <td>IDs de Gist permitidos. Se vazia, todos os Gists permitidos pela API.</td>
      <td>IDs separados por vírgula</td>
    </tr>
    <tr>
      <td><code>EXCLUDE_REPO</code></td>
      <td>Repositórios excluídos dos cartões de stats e linguagens sem expor nomes na URL pública. Útil com repos privados.</td>
      <td>Nomes de repositórios separados por vírgula</td>
    </tr>
    <tr>
      <td><code>FETCH_MULTI_PAGE_STARS</code></td>
      <td>Busca todas as páginas de stars para contagem correta (&gt;100 repos com estrela). Pode aumentar tempo e uso da API; na pública fica desligado.</td>
      <td><code>true</code> ou <code>false</code></td>
    </tr>
  </tbody>
</table>

Veja a [documentação da Vercel](https://vercel.com/docs/concepts/projects/environment-variables) sobre variáveis de ambiente.

> [!WARNING]
> Depois de alterar variáveis, faça **redeploy** para aplicar; deploys antigos não mudam sozinhos.

<h2 id="keep-your-fork-up-to-date">Manter o fork atualizado</h2>

Use o botão [Sync fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork) no GitHub ou automatize com o app [pull](https://github.com/wei/pull) ([@wei](https://github.com/wei)).

<h1 id="sparkling_heart-support-the-project">:sparkling_heart: Apoie o projeto original</h1>

O autor (Anurag Hazra) mantém muito código aberto e responde a quem precisa — isso leva tempo. O serviço público é gratuito.

Se este projeto te ajuda, você pode:

*   Dar crédito no README com link ao repositório. :D
*   Dar uma estrela e compartilhar. :rocket:
*   [![paypal.me/anuraghazra](https://ionicabizau.github.io/badges/paypal.svg)](https://www.paypal.me/anuraghazra) — doação única no PayPal (provavelmente vira chá :tea:).

Obrigado! :heart:

***

[![https://vercel.com?utm\_source=github\_readme\_stats\_team\&utm\_campaign=oss](powered-by-vercel.svg)](https://vercel.com?utm_source=github_readme_stats_team\&utm_campaign=oss)

Contribuições são bem-vindas! <3

Feito com :heart: e JavaScript.

---

**Forkado e traduzido por [@danvitoriano](https://github.com/danvitoriano).**
