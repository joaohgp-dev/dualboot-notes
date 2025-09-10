# Windows 11

### Navegação rápida

[[ Voltar ao início ]](../README.md#dual-boot---arch-linux--windows-11)  
[[ Pré instalação ]](./0-pre-install/README.md#windows-11--pré-instalação)  
[[ Instalação ]](./1-installation/README.md#windows-11--instalação)  
[[ Pós instalação ]](./2-post-install/README.md#windows-11--pós-instalação)

## Introdução

Esta seção agrupa os tópicos relacionados ao **Windows 11** para um ambiente de *dual boot* com **Arch Linux**. Serão abordados os passos necessários para preparar, instalar e configurar o sistema operacional.

## Sumário

* [Introdução](./README.md#introdução): Introdução da seção do Windows 11.
* [Pontos de partida](./README.md#pontos-de-partida): Detalha os diferentes cenários que o material cobre.
* [Recomendação do autor](./README.md#recomendação-do-autor): Recomendação do autor sobre qual método seguir em casos específicos.
* [Objetivos](./README.md#objetivos): Metas a serem alcançadas.

## Pontos de partida

Este material considera dois cenários:  

### Cenário 1 - Instalação limpa (RECOMENDADO)

> Ideal para aprender e realizar uma instalação limpa, organizada e otimizada.

Instruções para uma nova instalação do Windows 11, preparada para dual boot com Arch Linux.

* Prós: 
  * Controle sobre o particionamento; 
  * Menor chance de conflitos com o Arch Linux.  

* Contras: 
  * Apaga todos os dados do disco (é necessário fazer backup);
  * Requer mais tempo para reinstalação e configuração.

### Cenário 2 - Utilizar uma instalação existente

> Mais rápido, mas pode ter limitações.

Instruções para preparar uma instalação existente do Windows 11 para dual boot com Arch Linux.

* Prós: 
  * Preserva dados, programas e configurações atuais; 
  * Menos passos necessários.  

* Contras: 
  * Exige cuidados com redimensionamento de partições; 
  * Menos opções de recuperação em caso de erro.

### Recomendação do autor

Para quem deseja manter o Windows 11 como sistema principal e não se importa em usar o Arch Linux apenas em linha de comando, considere o [WSL2](./README.md#página-do-wsl2) como uma melhor alternativa. Para aqueles que buscam aprender e experimentar, reitero a recomendação de optar por uma instalação limpa.

## Objetivos - Cenário 1 (Instalação limpa)

### Pré instalação
* **Mídia de instalação**: Criar um dispositivo USB bootável com o Windows 11.
* **Arquivo de resposta**: Configurar um arquivo de resposta `autounattend.xml` para modificar a instalação e otimizar processos de configuração.
* **Opções do firmware**: Acessar o firmware do computador e alterar opções para permitir a instalação de ambos sistemas operacionais.

### Instalação
* **Instalar o Windows 11**: Realizar a instalação do sistema operacional, levando em consideração etapas realizadas na pré-instalação.

### Pós instalação
* **Configurar o sistema**: Ajustar as configurações do Windows 11, atualizar o sistema e otimizar opções.
* **Instalação de softwares**: Instalação e configuração de softwares essenciais.

## Objetivos - Cenário 2 (Instalação existente)

### Pós instalação
* **Gerenciamento de partições**: Redimensionar e reordenar partições do disco.
* **Ajuste de configurações do Windows 11**: Ajustar opções do Windows 11 para evitar problemas com o Arch Linux.
* **Opções do firmware**: Acessar o firmware do computador e alterar opções para permitir a instalação do Arch Linux.
* **Instalação de softwares**: Instalação e configuraçẽo de softwares essenciais.

## Referências
#### Página do WSL2
https://learn.microsoft.com/pt-br/windows/wsl/install