essa é a minha configuração pessoal do portage, feita especificamente pro x230.

ela é bem mínima, focada em:
- llvm profile/clang
- thin lto, -O3 
- USE="*-" desativado todas as use flags padrões
- sistema enxuto
- otimizações pensando no meu uso diário

## AVISO

**não use essa configuração. sério.**

ela foi feita pra minha máquina, meu hardware e minhas escolhas.
copiar isso sem entender pode:
- quebrar seu sistema
- causar erros estranhos de compilação
- gerar problemas difíceis de debugar
- fazer você perder tempo à toa

se algo aqui te inspirar, leia, entenda e tenta replicar. 
