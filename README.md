# ZOOP-POS-DEPENDENCY

Este repositório se destina a armazenar versões fixas das dependências dos mais variados tipos dos projetos da equipe de Devices: desde módulos e bibliotecas até ferramentas.

O repositório se divide nos seguintes subdiretórios:

- [`tools/`](#tools).

Outros subdiretórios sugeridos:

- `libraries/`;
- e `modules/`.

### Como usar este repositórios em _workflows_ do GitHub Actions?

Pode-se usar a _action_ [actions/checkout](https://github.com/actions/checkout/) para fazer o _checkout_ deste repositório em um _workflow_. Inclusive, pode-se até mesmo fazer o _checkout_ de uma versão específica deste repositório, indicando _branch_ ou _tag_, e/ou de arquivos específicos, indicando-os no filtro de _sparse checkout_.

| 💡 Dica |
| :--- |
| Consulte a página da _action_ [actions/checkout](https://github.com/actions/checkout/) para mais detalhes sobre como usá-la. |

---

## `tools/`

No subdiretório [`tools/`](./tools/), armazena-se ferramentas usadas nos projetos ou em processos pertinentes a esses.

### Adicionando novas ferramentas

Recomenda-se fortemente que cada conjunto de arquivos que compõem uma ferramenta seja armazenado na forma de um arquivo compactado (ex.: .zip, .tar, .gz, etc.). Além disso, é desejável que o número de versão — e a plataforma/o SO, se for o caso — sejam especificados no nome do arquivo. Por exemplo, se se deseja adicionar a versão v1.2.3 para Windows de uma ferramenta chamada _foo_, então se adiciona um arquivo compactado de nome `foo_windows_1.2.3.{extensão}` ou similar.
