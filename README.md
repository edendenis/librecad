# Como configurar/instalar o `LibreCAD` no `Linux`

## Resumo

Neste documento estão contidos os principais comandos e configurações para configurar/instalar o `LibreCAD` no `Linux`.

## _Abstract_

_In this document are contained the main commands and settings to set up/install the `LibreCAD` on `Linux`._

## Descrição [2]

`LibreCAD`

O `LibreCAD` é uma aplicação de código aberto de desenho técnico e modelagem 2D, projetada para criar projetos e desenhos técnicos em sistemas operacionais Unix-like, incluindo Linux. Inspirado pelo software AutoCAD, o `LibreCAD` oferece uma variedade de recursos de desenho precisos, como criação de linhas, círculos, arcos e polígonos, além de ferramentas de edição e dimensionamento. Ele é frequentemente usado por engenheiros, arquitetos e projetistas para criar plantas baixas, esquemas técnicos e desenhos detalhados. O `LibreCAD` é uma opção gratuita e de código aberto que fornece uma alternativa acessível para aqueles que buscam uma ferramenta de CAD 2D para atender às suas necessidades de design técnico.


## 1. Como configurar/instalar o `LibreCAD` no Linux [1]

Para configurar o `LibreCAD`, você pode seguir estas etapas:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`

2. Certifique-se de que seu sistema esteja limpo e atualizado.

    2.1 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.2 Remover pacotes `.deb` antigos ou duplicados do cache local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando: `sudo apt autoclean`

    2.3 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando: `sudo apt autoremove -y`

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`: `sudo apt update`

    2.5 **Corrigir pacotes quebrados**: Isso atualizará a lista de pacotes disponíveis e tentará corrigir pacotes quebrados ou com dependências ausentes: `sudo apt --fix-broken install`

    2.6 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.7 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:  `sudo apt list --upgradable`

    2.8 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update`. Digite o seguinte comando e pressione `Enter`: `sudo apt full-upgrade -y`
    

Para instalar o `LibreCAD` através do terminal no `Linux`, o processo pode variar ligeiramente dependendo da distribuição que você está utilizando. Aqui estão as instruções para algumas das distribuições mais comuns:

3. **`Ubuntu` ou `Debian` e derivados:** `sudo apt install librecad -y`

Estes comandos instalarão a versão do `LibreCAD` disponível nos repositórios oficiais da sua distribuição Linux. Se você estiver usando uma distribuição que não está listada aqui, o processo será similar, mas o gerenciador de pacotes pode ser diferente (por exemplo, yum no lugar de apt para distribuições baseadas em Red Hat mais antigas).

Após a instalação, você pode iniciar o `LibreCAD` a partir do seu menu de aplicativos ou executando librecad no terminal.

### 1.1 Codigo completo para configurar/instalar

Para instalar o `LibreCAD` no Linux sem precisar digitar linha por linha, você pode seguir estas etapas:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`

2. Digite o seguinte comando e pressione `Enter`:

    ```
    sudo apt clean                                                            
    sudo apt autoclean
    sudo apt autoremove -y
    sudo apt update
    sudo apt --fix-broken install
    sudo apt clean
    sudo apt list --upgradable
    sudo apt full-upgrade -y
    sudo apt install librecad -y
    librecad
    ```


## Referências

[1] OPENAI. ***FreeCAD e arquivos .prt no Linux.*** Disponível em: <https://chat.openai.com/c/4d66a3c1-dae0-4cf5-b9fb-3e4e2979a61e> (texto adaptado). ChatGPT. Acessado em: 29/01/2024 10:06.

[2] OPENAI. ***Vs code: editor popular*** Disponível em: <https://chat.openai.com/c/b640a25d-f8e3-4922-8a3b-ed74a2657e42>s (texto adaptado). ChatGPT. Acessado em: 29/01/2024 10:06.
