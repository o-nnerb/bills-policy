# Bills — Política de Privacidade e Termos de Uso

Documentos públicos do app **Minhas Contas: Orçamentos (Bills)**. / Public documents of the **Bills (Minhas Contas: Orçamentos)** app.

**Site: <https://o-nnerb.github.io/bills-policy/>**

| | Português | English |
|---|---|---|
| Política de Privacidade / Privacy Policy | [Privacidade](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacidade/) | [Privacy](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy/) |
| Termos de Uso / Terms of Use | [Termos](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/termos/) | [Terms](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms/) |

### Outros idiomas / Other languages

As traduções para os idiomas abaixo foram feitas por IA a partir do texto em inglês e ainda não foram revisadas por advogados nem por falantes nativos. Idiomas sem tradução usam as páginas em inglês. / The translations below were made by AI from the English text and have not yet been reviewed by lawyers or native speakers. Languages without a translation use the English pages.

| Idioma / Language | Privacidade / Privacy | Termos / Terms |
|---|---|---|
| Español | [Privacy-es](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-es/) | [Terms-es](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-es/) |
| Français | [Privacy-fr](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-fr/) | [Terms-fr](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-fr/) |
| Deutsch | [Privacy-de](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-de/) | [Terms-de](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-de/) |
| Italiano | [Privacy-it](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-it/) | [Terms-it](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-it/) |
| 日本語 | [Privacy-ja](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-ja/) | [Terms-ja](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-ja/) |
| 한국어 | [Privacy-ko](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-ko/) | [Terms-ko](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-ko/) |
| 简体中文 | [Privacy-zh-Hans](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-zh-hans/) | [Terms-zh-Hans](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-zh-hans/) |
| 繁體中文 | [Privacy-zh-Hant](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-zh-hant/) | [Terms-zh-Hant](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-zh-hant/) |
| Русский | [Privacy-ru](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-ru/) | [Terms-ru](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-ru/) |
| العربية | [Privacy-ar](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-ar/) | [Terms-ar](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-ar/) |
| Türkçe | [Privacy-tr](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-tr/) | [Terms-tr](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-tr/) |
| Nederlands | [Privacy-nl](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-nl/) | [Terms-nl](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-nl/) |
| Polski | [Privacy-pl](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-pl/) | [Terms-pl](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-pl/) |
| Bahasa Indonesia | [Privacy-id](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-id/) | [Terms-id](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-id/) |
| हिन्दी | [Privacy-hi](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy-hi/) | [Terms-hi](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms-hi/) |

Cada página tem, logo abaixo da data de vigência, a lista de idiomas para trocar de versão. / Each page has the language list right below the effective date.

Dúvidas ou pedidos: <o.nnerb@icloud.com> ou uma [issue](https://github.com/o-nnerb/bills-policy/issues). / Questions or requests: <o.nnerb@icloud.com> or an [issue](https://github.com/o-nnerb/bills-policy/issues).

O histórico de mudanças dos documentos é o histórico de commits deste repositório. / The change history of the documents is the commit history of this repository.

## Como o site é gerado

Os textos estão em [`BillsPolicy.docc`](BillsPolicy.docc), um catálogo do [DocC](https://www.swift.org/documentation/docc/) só com artigos. O workflow [`docs.yml`](.github/workflows/docs.yml) roda `docc convert` e publica no GitHub Pages a cada push para `main`; em pull request só compila (e falha se o DocC gerar avisos, como um link quebrado).

Para ver localmente (precisa do Xcode):

```bash
xcrun docc preview BillsPolicy.docc --fallback-display-name BillsPolicy --fallback-bundle-identifier br.com.onnerb.BillsPolicy --experimental-enable-custom-templates
```

O arquivo [`header.html`](BillsPolicy.docc/header.html) (que exige a flag `--experimental-enable-custom-templates`, já usada no workflow) faz o navegador escolher a direção de cada parágrafo pelo próprio texto, para as páginas em árabe aparecerem da direita para a esquerda.

Para cada idioma há dois arquivos, `Privacy-<código>.md` e `Terms-<código>.md` (`<código>` = es, fr, de, it, ja, ko, zh-Hans, zh-Hant, ru, ar, tr, nl, pl, id, hi), com os mesmos títulos e a mesma ordem do inglês. Ao adicionar um idioma, inclua-o também nos tópicos de [`BillsPolicy.md`](BillsPolicy.docc/BillsPolicy.md) e na lista de idiomas no topo de cada página.

Se mudar o sentido de um texto, atualize a data de vigência no topo da página (em todos os idiomas) e o app deve avisar quem já usa.
