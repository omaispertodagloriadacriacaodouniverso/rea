# Rota própria (fork independente — sem esperar upstream)

Direção nossa, não deles. Upstream vira referência (cherry-pick), não dono.

## Alvos

1. Setup opencode-first (detecção/config sem Claude-centrismo).
2. PT-BR real nas docs de uso (não só README).
3. Integração evidência→relatório (modelo `rea-relatorio` do nosso pack).
4. Pin local das versões homologadas por nós.

## Regras

- Branch `nossa/` p/ linha própria; `fix/` só p/ PRs upstream ocasionais.
- Todo diff aqui passa na suíte deles (`vitest run` no que tocar) + a nossa.
