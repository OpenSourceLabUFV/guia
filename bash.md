# Bash

Bash é uma interface de linha de comando - também chamada de **shell** - e uma linguagem de script. Na (grande) maioria das distribuições Linux ela é a forma padrão de interagir com o sistema. Existem outras shells, como por exemplo a ZSH, que é padrão nas versões recentes do MacOS. Ela também entende a linguagem Bash, então é basicamente uma questão de preferência pessoal.

No Windows, é possível usar a linguagem Bash através do Windows Subsystem for Linux, além de poder usar qualquer Shell de sua preferência.

Se você for escrever algum script necessário para algum projeto, recomendamos a linguagem Bash por estar disponível na maioria das plataformas e facilitar a colaboração.

Se você nunca usou Bash, um excelente tutorial de introdução pode ser encontrado [aqui](https://swcarpentry.github.io/shell-novice/). Caso já tenha alguma experiência, falarei aqui um pouco sobre o uso interativo e em scripts.

## Uso Interativo

Bash tem diversos atalhos de teclado, e alguém já fez um maravilhoso post introdutório [aqui](https://www.tecmint.com/linux-command-line-bash-shortcut-keys/). Esses atalhos são muito úteis já que tudo no terminal é feito através do teclado.

Uma outra funcionalidade muito interessante do Bash são as **aliases**. Basicamente, você pode dar nomes para comandos que você usa frequentemente, salvando assim tempo de digitação. Alguém também já fez um post muito bom sobre isso [aqui](https://linuxize.com/post/how-to-create-bash-aliases/), então se quiser saber mais é só acessar o link.

### Ferramentas comuns

Existem algumas ferramentas de linhad e comando muito utilizadas. Você pode sempre usar a internet ou usar o comando `man` para ler o manual dela no terminal, mas vou listar algumas muito úteis que podem salvar muito tempo caso você já saiba.

#### Arquivos

* `ls` - Lista arquivos e pastas
* `tree` - Dá uma representação gráfica da estrutura de uma pasta
* `cd` - Muda a pasta atual
* `pwd` - Mostra o diretório atual
* `cp` - Copia um arquivo para outra pasta
* `mv` - Move um arquivo para outra pasta
* `rm` - Remove um arquivo ou uma pasta
* `mkdir` - Cria uma nova pasta
* `touch` - Cria um novo arquivo em branco
* `chmod` - Muda as permissões de um arquivo ou pasta
* `chown` - Muda o dono de um arquivo ou pasta
* `find` - Procura por arquivos ou pastas no sistema
* `locate`, `updatedb` - Procura por arquivos ou pastas usando um banco de dados
* `tar` - Manipula arquivos .tar ou .tar.gz
* `zip` - Decompacta arquivos .zip
* `df` - Mostra o espaço vazio no disco
* `du` - mostra o uso de disco de arquivos e pastas

### Programas

* `man` - Leia o manual
* `ps` - Mostra todos os programas que estão sendo executados
* `top` - O mesmo do `ps`, porém de forma interativa
* `kill` - Para um programa
* `which` - Descubra qual arquivo será executado quando rodar um comando

### Sistemas Remotos

* `ssh` - Conecta a uma shell em um computador remoto
* `rsync` - Copia arquivos entre computadores usando SSH
* `lftp` - Copia arquivos entre computadores usando FTP
* `wget`, `curl` - Copia arquivos usanfo requisições https ou a APIs
* `who` - Mostra quem está logado

Se quiser saber mais, você pode encotrar [aqui](https://fossbytes.com/a-z-list-linux-command-line-reference/) uma lista (muito) extensa de comandos.

## Scripts

É possível escrever código em bash e salvar em um arquivo para facilitar o uso de uma cadeia de comandos que você usa normalmente.

Porém, só recomendamos escrever scripts em bash quando for realmente necessário. Existem diversas outras linguagens de script por aí - como Python - que são linguagens com muito mais recursos e bibliotecas, e podem facilitar seu desenvolvimento.

Portanto, prefira usar bash para comandos rápidos no próprio terminal, e não para escrever scripts. Porém, caso precise, sempre use o [shellcheck](https://www.shellcheck.net/) para ter certeza que seu script faça o que você quer.