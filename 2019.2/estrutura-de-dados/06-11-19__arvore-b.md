# Ávore B - 06/11/19

Inclusão | Remoção
--- | ---
Descer a partir da raiz sempre entrando em nó cheio. | Descer a partir da raiz sempre entrando em nó "não pequeno" [ n[x] >= t ] (= não é (t - 1)).

**OBS:** raiz[T] não é pequena.
1 <= n  [ raiz[T] ] <= 2tn - 1

## Algorítmo: Remover chave K de subárvore enraizada em `x` [x não é pequeno] em árv. B

Inicialmente, remover k de raiz[t].

1. Se k está em x e x é folha (x não é pequeno), remova k de x.
2. Se k está em x e x não é folha, faça:
   1. Se n[y] >= t, remover predecessor k' de k (de y) e substituir k por k'.
   2. Se n[z] >= t, remover sucessor k' de k (de z) e substituir k por k'.
   3. Se ambos possuem t - 1 chaves (n[y] = t -1 e n[z] = t - 1), fazer merge de y com z e remover k do novo filho.
3. Se k não está em x e x é nó interno. (se x é folha, k não está na subárvore enraizada em x e não há nada a fazer).
   1. Se n[fi[x]] >= t (se esse filho não é pequeno), remover k da subárvore enraizada em fi[x].
   2. Se n[fi[x]] = t - 1 (secesse filho é pequeno), mas este nó possui um irmão imediato com pelo menos t chaves (>= t): pegar chave emprestada do irmão e remover k do nó fi[x].
   3. Se n[fi[x]] = t - 1 mas este nó possui irmão imediato  com t - 1 chaves: fazer mrtge com irmão e remover k do novo nó criado.

**Custo por nível:**

Custo | Operaçoes de disco | RAM
--- | --- | ---
Por nível | O(1) | O(t)
Total | O(log(n) na base t) | O(t * log(n) na base t)
