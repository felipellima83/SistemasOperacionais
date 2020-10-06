# SistemasOperacionais
Repositório criado para o desenvolvimento do SO CeubOS


CENTRO DE ENSINO UNIFICADO DE BRASÍLIA - UniCEUB
FACULDADE DE TECNOLOGIA E CIÊNCIAS SOCIAIS APLICADAS
CURSO DE CIÊNCIAS DA COMPUTAÇÃO
DISCIPLINA SISTEMAS OPERACIONAIS








DOCUMENTAÇÃO BÁSICA
COMO INICIAR O CEUB-OS A PARTIR DE UM PENDRIVE









Autor:
Felipe Ferreira Lima e Lima







Brasília, DF (2020)
APRESENTAÇÃO
Para que um computador funcione como conhecemos, é necessário que ele possua vários softwares previamente instalados, pois sem eles um computador é inútil, e um dos principais é o sistema operacional (SO).
Mas o que vem a ser um sistema operacional? 
“O programa de sistema mais básico é o sistema operacional, cuja tarefa é controlar todos os recursos do computador e fornecer uma base sobre a qual os programas aplicativos podem ser escritos” (Tanenbaum, 2008, p.21). 
De acordo com Barreto (UFSC, sem data)
O SO é o conjunto de programas que gerenciam recursos, processadores, armazenamento, dispositivos de entrada e saída e dados da máquina e seus periféricos. O sistema que faz comunicação entre o hardware e os demais softwares. O Sistema Operacional cria uma plataforma comum a todos os programas utilizados. Exemplos: DOS, Unix, Linux, Mac OS, OS-2, Windows NT.
Vemos, de acordo com acima descrito, a importância de uma instituição de ensino do porte do Centro Universitário de Brasília - UniCEUB em possuir uma distribuição de um sistema operacional para manter o controle das informações que são ali produzidas pelos alunos, professores e administração, e para isso, foi utilizado o linux como base no desenvolvimento de tal sistema, que foi nomeado como CEUB-OS.
O Linux foi utilizado como base devido a ser o SO mais utilizado no mundo, ultrapassando até mesmo o conhecidíssimo Windows em suas diversas versões. Porém o motivo principal é devido ao Linux não ter sido desenvolvido com fins comerciais, sendo seu código fonte aberto a todos que queiram modificar ou criar novas distribuições a partir dele.
A idéia de desenvolver um SO específico para o UniCEUB partiu do pressuposto que nem todos os alunos possuem um computador potente que consiga rodar qualquer SO. Como o Linux é altamente personalizável, a idéia foi de deixá-lo o mais enxuto possível, como os softwares básicos necessários ao desenvolvimento dos estudos das diversas disciplinas de qualquer curso presente na instituição.
OBJETIVO
Esse trabalho foi desenvolvido com o intuito de apresentar e esclarecer para pessoas leigas o que é o CEUB-OS e sua importância para disciplina Sistemas Operacionais, dando ênfase em como fazer o download, preparar e iniciar o CEUB-OS a partir de um pendrive em modo live.
INSTRUÇÕES E MANUAIS
Os usuários de computadores quando escutam a palavra Linux, a primeira impressão que vem a suas cabeças é a de que ele é um SO de difícil operação, com uma interface nada fácil de ser aprendida e que não deve ser utilizado por pessoas que não tem conhecimento avançado em informática e seus desdobramentos.
No entanto, hoje, pode-se ver que existem diversas versões do Linux, que possuem diferentes interfaces gráficas modernas e de fácil utilização e o CUB-OS é uma dessa versão.
Caso o usuário não queira instalar o CEUB-OS em sua máquina e perder o seu SO já instalado, ele tem a opção de construir uma versão live que não precisar ser instalado na máquina e sim utilizado apenas um pendrive. E para efetivar tal função é necessário utilizar alguns outros softwares como baixar a versão mais atual do CEUB-OS.
É necessário um pendrive com no mínimo 8GB para utilização do CEUB-OS em sua versão Live.
Para fazer o download da última versão do CEUB-OS, deve-se clicar ou digitar em seu navegador o link https://sourceforge.net/projects/ceubos/files/build/ e posteriormente clicar no ícone “Donwload Latest Version”, conforme indicado pelo retangulo vermelho na imagem 01 abaixo. É extremamente aconselhável utilizar a última versão disponibilizada.
Imagem 01 - Local de download da última versão do CEUB-OS

Após concluída a etapa anterior, o próximo software a ser efetuado o download e instalado é o Linux Live USB Creator, disponível no link https://www.linuxliveusb.com/. Depois de clicar no ícone “Downloads”, conforme mostrado na imagem 02, marcado com o retângulo vermelho, uma nova janela abrirá e agora basta clicar em “Download LiLi”, conforme mostrado na imagem 03, que o download iniciará automaticamente.
Imagem 02 - Site para Download Linux Live USB Creator


Imagem 03 - Download Linux Live USB Creator

Ao término do download, basta instalar o software seguindo as orientações apresentadas no instalador. Não tem segredo, elas estão em português para facilitar!
Continuando com os procedimentos, inicie o LiLi USB Creator, sua interface é na versão utilizada aqui igual ao apresentado na imagem 04 abaixo.

Imagem 04 - Linux Live USB Creator e suas opções

Para começar, insira o pendrive em uma porta usb do seu computador, depois, no “PASSO 1: ESCOLHER UMA PENDRIVE”, escolha a porta do pendrive que irá instalar o SO. Depois de escolhido o pendrive, vá em “PASSO 2 : ESCOLHER A FONTE” e selecione ISO/IMG/ZIP, uma janela se abrirá para selecionar o arquivo ISO do CEUB-OS anteriormente baixado. Selecione o arquivo no local onde foi salvo a ISO e clique em selecionar. Realizado os passos anteriores, no “PASSO 4 : OPÇÕES”, selecione as três opções disponíveis, e para finalizar a instalação clique no raio amarelo em “PASSO 5 : INSTALAÇÃO”. Aguarde o tempo necessário para concluir a instalação.
Agora que tudo já foi devidamente instalado, partiremos para a parte onde iremos configurar o computador para iniciar o CEUB-OS assim que o computador for ligado. Ao ligar o computador, será necessário entrar na BIOS para desabilitar o secure boot.
Como existem BIOS de diferentes marcas, o procedimento aqui mostrado é apenas de referência e, por isso, qualquer detalhamento mais profundo (como a tecla de acesso à BIOS e outros), deve ser consultado o manual do PC, na parte que fala sobre a placa mãe ou entre em contato com o suporte do fabricante do computador. CUIDADO!!! As alterações devem ser feitas com muito cuidado e por sua própria conta e risco.
Segundo o site Profissionais TI (Como desabilitar a opção de Boot Seguro UEFI, 2013)
Para acessar a BIOS do computador, a tecla de atalho usada geralmente é a Del (delete). Ao reiniciar o computador, já na primeira tela, irá aparecer a tecla de atalho correspondente para entrar na Bios. 
Ao entrar na BIOS, terá que localizar a opção correspondente ao Secure Boot (inicialização segura), desativá-la e alterar a opção referente ao UEFI para a opção Legacy.
Após alterar estas opções, altere a sequência de Boot do seu sistema para o dispositivo referente à leitora de DVD, caso for instalar o novo sistema via mídia de DVD, ou coloque como primeira opção para o seu dispositivo USB, caso for instalar via pen drive, ou então pelo dispositivo network, caso for instalar via rede. Agora basta salvar as configurações da Bios usando a tecla F10, que é a tecla de  atalho usada normalmente para esta função, e ao reiniciar o computador, fazer a instalação do Sistema Operacional como de costume.
Imagem 05 - Desativando o boot seguro

Ao término das configurações indicadas, desligue o computador, insira o pendrive em um entrada USB, liguei o computador novamente e comece a pressionar a tecla de boot (F2 na maioria dos casos) e em seguida selecione a opção USB.
Pronto, agora é só seguir as orientações de instalação, que basicamente é escolher o idioma, e começar a utilizar o seu sistema operacional CEUB-OS.
CONCLUSÕES
Com base nas informações passadas ao longo deste “manual”, pode ser verificado que tal procedimento de rodar um sistema operacional em um pendrive em modo live não é difícil, basta apenas saber onde encontrar os softwares e o sistema operacional para serem baixados e seguir as orientações aqui passadas.
Outro ponto de relevância, é a agilidade que o sistema desenvolvido apresenta, pois até mesmo rodando em um pendrive ele é extremamente rápido e estável.
REFERÊNCIAS BIBLIOGRÁFICAS
Barreto, Jorge Muniz. Universidade Federal de Santa Catarina. Departamento de Informática e Estatística. Disponível em: https://www.inf.ufsc.br/~j.barreto/cca/sisop/sisoperac.html. Acesso em: 02 out. 2020.
Como desabilitar a opção de Boot Seguro UEFI. Profissionais TI. Disponível em: https://www.profissionaisti.com.br/desabilitando-a-opcao-de-boot-seguro-uefi/. Acesso em: 02 out. 2020.
Linux Live USB Creator. Disponível em: https://www.linuxliveusb.com/. Acesso em: 02 out. 2020.
Sistemas operacionais [recurso eletrônico] : projeto e implementação / Andrew S. Tanenbaum, Albert S. Woodhull ; tradução João Tortello. – 3. ed. – Dados eletrônicos. – Porto Alegre : Bookman, 2008.

