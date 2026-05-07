# Pokédex

Aplicação estática em HTML, CSS e JavaScript para explorar dados da [PokéAPI](https://pokeapi.co/).

## Visão Geral

O projeto exibe:

- Lista de Pokémon com busca, filtro por tipo e modal de detalhes
- Exploradores separados para tipos, movimentos, habilidades, itens, regiões e gerações
- Paginação nas listas principais

## Estrutura

- `public/index.html` - página principal da Pokédex
- `public/explorer-types.html` - explorador de tipos
- `public/explorer-moves.html` - explorador de movimentos
- `public/explorer-abilities.html` - explorador de habilidades
- `public/explorer-items.html` - explorador de itens
- `public/explorer-regions.html` - explorador de regiões
- `public/explorer-generations.html` - explorador de gerações
- `netlify.toml` - configuração de deploy para Netlify

## Requisitos

- Navegador moderno
- Conexão com a internet para consultar a PokéAPI e os recursos externos do Bootstrap e Google Fonts

## Rodando Localmente

Você pode abrir os arquivos diretamente no navegador, mas o ideal é servir a pasta `public` como raiz do site.

Exemplo com servidor local simples:

```bash
python -m http.server 8000 --directory public
```

Depois abra:

- `http://localhost:8000`

## Deploy no Netlify

O projeto já vem preparado para Netlify.

Configuração usada:

- `publish = "public"`

Isso faz o Netlify publicar a pasta `public` como raiz do site.

## Funcionalidades

- Busca por nome e número de Pokémon
- Filtro por tipo
- Paginação de resultados
- Modal com dados completos do Pokémon
- Modais de detalhes para tipos, movimentos, habilidades, itens, regiões e gerações

## API

O projeto usa a versão 2 da PokéAPI:

- `https://pokeapi.co/api/v2/`

## Observações

- As páginas dependem de requisições externas à PokéAPI.
- Alguns exploradores carregam listas grandes de dados e podem demorar um pouco na primeira abertura.
