# 🔥 Tinder Imob — WB Negócios Imobiliárias

Painel interativo de **match entre a demanda do cliente e a carteira de captações** da imobiliária.
Cruza oferta (imóveis ativos) e demanda (o que o cliente procura) e ranqueia os imóveis por
compatibilidade — com interface de **cards estilo Tinder** e **ranking** analítico.

> Aplicação de arquivo único: basta abrir o `TINDER_IMOB.html` no navegador (funciona offline,
> sem servidor e sem instalação).

## ✨ Funcionalidades

- **Cadastro de demanda**: finalidade, tipo de imóvel, área mínima, dormitórios, suítes, vagas,
  bairro(s) e faixa de orçamento.
- **Score inteligente (0–100)** — pesos: orçamento 30 · bairro 20 · dormitórios 20 · área 15 ·
  suítes 8 · vagas 7. Área/dormitórios/suítes/vagas contam como **mínimos**, valor como **teto** e
  bairro como **preferência** (bairros da mesma região pontuam parcialmente → mostra "quase-matches").
- **Cards estilo Tinder**: deslize ❤️ (favoritar) / ✕ (descartar), com botões e setas do teclado.
- **Ranking**: tabela ordenável por match, valor, área, dormitórios etc.
- **Favoritos (shortlist)**: exportação em **CSV** e **impressão/PDF** para enviar ao cliente.
- **Histórico de buscas**: ao limpar os filtros ou arquivar, a shortlist atual vira um **card
  colapsável** no histórico (com cliente, resumo da demanda, restaurar, exportar e excluir).
- **Persistência local** (localStorage): favoritos e histórico continuam salvos ao reabrir.
- **Filtros rígidos opcionais**: "somente dentro do orçamento", "somente bairros selecionados" etc.

## 🚀 Como usar

1. Abra `TINDER_IMOB.html` no navegador (duplo clique).
2. Preencha a **demanda do cliente** no painel da esquerda.
3. Clique em **🔥 Encontrar matches** e deslize pelos cards ou veja o **Ranking**.
4. Favorite os melhores, exporte a **shortlist** em CSV/PDF e envie ao cliente.

## 🗂️ Dados

A carteira é um **snapshot** exportado da Kenlo Imob (203 imóveis ativos · 23/06/2026), embutido no
próprio HTML. Para atualizar: reexporte a planilha de imóveis da Kenlo e gere uma nova versão do painel.

Imóveis com preço de venda inconsistente no cadastro aparecem marcados como **"a confirmar"**.

---
Feito com auxílio do Claude (Cowork). Uso interno da imobiliária.
