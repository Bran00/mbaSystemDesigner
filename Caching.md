## Caching

- Aplication -> Cache
             <-
- Database

------------------------------------

- Time-based invalidation
- Least Recently Used(LRU)
- Most Recently Used(MRU)
- Least Frequently Used(LFU)
- TTL-based invalidation
- Write-through invalidation
- Write-back invalidation

Caching - LRU

C*
B
A

Caching - MRU

A Remove a atual
B E pega a A atualizada

Caching - LFU

Remove o menos acessado

D - 10
C - 5*
B - 6
A - 7

Caching - Write-through invalidation
Sempre quando há alteração no disco, o cache é atualizado em conjunto.
Essa estratégia funciona bem com sistema com pouca escrita.

Caching - Write-back invalidation

Quando há alteração, o cache primeiramente é atualizado e depois o dado em disco é atualizado. Muitas vezes o dado em disco é atualizado quando o cache já está para expirar de alguma forma.
