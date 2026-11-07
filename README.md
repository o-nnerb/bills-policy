# Bills — Política de Privacidade e Termos de Uso

Documentos públicos do app **Minhas Contas: Orçamentos (Bills)**. / Public documents of the **Bills (Minhas Contas: Orçamentos)** app.

**Site: <https://o-nnerb.github.io/bills-policy/>**

| | Português | English |
|---|---|---|
| Política de Privacidade / Privacy Policy | [Privacidade](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacidade/) | [Privacy](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/privacy/) |
| Termos de Uso / Terms of Use | [Termos](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/termos/) | [Terms](https://o-nnerb.github.io/bills-policy/documentation/billspolicy/terms/) |

Dúvidas ou pedidos: <o.nnerb@icloud.com> ou uma [issue](https://github.com/o-nnerb/bills-policy/issues). / Questions or requests: <o.nnerb@icloud.com> or an [issue](https://github.com/o-nnerb/bills-policy/issues).

O histórico de mudanças dos documentos é o histórico de commits deste repositório. / The change history of the documents is the commit history of this repository.

## Como o site é gerado

Os textos estão em [`BillsPolicy.docc`](BillsPolicy.docc), um catálogo do [DocC](https://www.swift.org/documentation/docc/) só com artigos. O workflow [`docs.yml`](.github/workflows/docs.yml) roda `docc convert` e publica no GitHub Pages a cada push para `main`; em pull request só compila (e falha se o DocC gerar avisos, como um link quebrado).

Para ver localmente (precisa do Xcode):

```bash
xcrun docc preview BillsPolicy.docc --fallback-display-name BillsPolicy --fallback-bundle-identifier br.com.onnerb.BillsPolicy
```

Se mudar o sentido de um texto, atualize a data de vigência no topo da página e o app deve avisar quem já usa.
