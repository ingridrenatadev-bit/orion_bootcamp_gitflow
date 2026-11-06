# 📚 Guia de Aprendizado: Git e Gitflow

## 🌿 Entendendo o Gitflow
O **Gitflow** é um modelo de ramificação (branching) estruturado que define um ciclo de vida rígido para o lançamento de software e organiza a colaboração de forma previsível. 

Abaixo estão os principais tipos de branches que utilizamos neste fluxo:

| Branch | Descrição e Propósito |
| :--- | :--- |
| `production` (ou `main`/`master`) | Branch oficial que contém o código em **produção** |
| `stage` (ou `staging` / `release`) | Ambiente de homologação ou testes finais antes de subir para a produção. |
| `develop` | Branch de integração para o desenvolvimento de novas funcionalidades. É a base para as novas branches de `feature`. |
| `feature/*` | Branches criadas a partir da `develop` para desenvolver **novas funcionalidades** ou melhorias. Ao terminar, retornam para a `develop` via Pull Request. |
| `bugfix/*` | Branches para correção de **bugs encontrados na develop** antes de irem para o ambiente de testes/produção. |
| `hotfix/*` | Branches criadas diretamente da `production` para corrigir **erros críticos e urgentes** em ambiente de produção, sendo mescladas de volta para `production` e `develop`. |

---
