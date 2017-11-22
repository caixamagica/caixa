# Caixa Mágica

A Caixa Mágica é um dispositivo de código-aberto focado em facilitar processos democráticos e de participação cidadã. O projeto é desenvolvido por uma rede de colaboradores presentes no Brasil, Colômbia, México e Espanha. 

Saiba mais em: [caixamagi.ca](http://caixamagi.ca) (em construção)

### Como é feita a Caixa Mágica?

A Caixa Mágica é baseada em soluções de hardware e softwares acessíveis e, quando possíveis, de código-aberto. 

 **Hardware utilizado**
 - Raspberry Pi 3
 - TP Link Router MR3020
 - Cartão SD - mínimo 16 GB
 - Bateria externa (PowerBank) com 2 duas entradas USB

**Imagem (ISO) do sistema**
[Versão alpha](https://www.dropbox.com/s/d33vweaucp0c8ce/caixamagica.img?dl=0)
 
**Software utilizado**
 - LAMP (GNU/Linux Debian, Apache, MySQL, PHP)
 - [Aplicativo de deliberação da Caixa Mágica](https://github.com/OpenlabsCdMX/CaixaMagica)
 - [Aplicativo de priorização da Caixa Mágica](https://github.com/caixamagica/caixa-avaliacaolabicbr)

**Senhas utilizadas**
SSH: pi@192.168.0.1 | raspberry
MySQL: root | root | db name: caixa_magica


### Como montar uma Caixa Mágica com a ISO? 

 1. Grave a imagem da última versão da Caixa Mágica no cartão SD. Você pode utilizar programas como o [Etcher](http://etcher.io) para fazer isso. Depois de concluído o processo, insira o cartão SD na sua Raspberry Pi.
 2. Conectar o roteador à Raspberry Pi com um cabo ethernet e à bateria externa com o cabo USB.
 3. Conecte o Raspberry Pi na bateria e aguarde alguns minutos para a inicialização do sistema.
 4. Se tudo der certo, deverá ser criada uma rede WiFi chamado 'Caixa Mágica'. Agora, basta conectar a ele e, se o portal da Caixa Mágica não abrir automaticamente, abra seu navegador e busque a URL http://magia.caixamagica.eu
 

### Como armar una Caja Magica con la ISO?

 1. Grabar la imagen de la [ultima versión de 'Caixa Magica'](https://www.dropbox.com/s/d33vweaucp0c8ce/caixamagica.img?dl=0) en la tarjeta SD. Puedes utilizar softwares como o [Etcher](http://etcher.io) para eso. Basta descargar el fichero, abrir Etcher y seleccionar la imagen ISO y la tarjeta. Despues de completo el proceso, insira la tarjeta SD en tu Raspberry Pi.
 
 2. Conectar el router a la Raspberry Pi con un cabo ethernet y a la bateria externa com en el cabo USB.
 
 3. Conectar la Raspberry Pi en la bateria y aguardar algunos minutos para el sistema inicializar.
 
 4. Si todo va bien, ahora tienes una red WiFi llamada 'Caixa Mágica'. Ahora, conectate y, si el portal no abre automaticamente, con tu browser entre directamente en la URL http://magia.caixamagica.eu

 5. Selecione la opción 'Editar' en el 'Listado de Caixa' y modifique las perguntas

### Como montar uma Caixa Mágica desde o zero?

(Em construção...)

1. Instale o Debian em sua Raspberry Pi, configure o MySQL, Apache e PHP

2. Crie o portal captivo baixando o arquivo 'iptables.ipv4.nat' e inserindo-o no diretório '/etc'

3. Chame o arquivo 'iptables.ipv4.nat' no /etc/network/interfaces

