essa é a minha configuração pessoal do portage, feita especificamente pro x230.

ela é bem mínima, focada em:
- llvm profile/clang
- thin lto, -O3 
- USE="*-" desativado todas as use flags padrões
- sistema enxuto
- otimizações pensando no meu uso diário

## AVISO

**não copie essa configuração. sério.**

copiar isso sem entender pode:
- quebrar seu sistema (so tem firmwares para o x230)
- causar erros estranhos de compilação
- gerar problemas difíceis de debugar
- fazer você perder tempo à toa

use isso como inspiracão, entenda o uso das coisas e replique no seu sistema :)

