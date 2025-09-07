# Windows 11 \ Pré-instalação

## Introdução

Esta seção engloba os procedimentos realizados na pré-instalação do **Windows 11** para um ambiente de *dual boot* com **Arch Linux**.

## Objetivos

* **Mídia de instalação**: Criar um dispositivo USB bootável com o Windows 11.
* **Arquivo de resposta**: Configurar um arquivo de resposta `autounattend.xml`.

**Sumário**

* [Introdução](./README.md#introdução): Introdução da seção do Windows 11.
* [Objetivos](./README.md#objetivos): Metas a serem alcançadas.
* [Mídia de instalação](./README.md#mídia-de-instalação): Instruções para o preparo da mídia de instalação.
* [Arquivo de resposta](./README.md#arquivo-de-respota): 
* [Referências](./README.md#referências): Lista de referências.

## Mídia de instalação

O primeiro passo é baixar o arquivo de imagem do Windows 11 e preparar um dispositívo USB. A imagem original está disponível na [página de download](#página-de-download-do-windows-11) da Microsoft.  
O segundo passo é baixar e instalar um software que prepare a mídia de instalação USB, geralmente um pen drive. Exemplos de software para Windows são o [**Microsoft Media Tool**](#página-de-download-do-windows-11) e [**Rufus**](#página-do-rufus), para Linux o [**WoeUSB**](#página-do-woeusb).

> [!WARNING]  
> Para evitar conflitos, não utilize as opções avançadas do **Rufus**, visto que posteriormente usaremos outro método para personalizar a instalação.

O terceiro passo é utilizar o software escolhido para preparar uma mídia de instalação do Windows 11.  

## Arquivo de respota

O arquivo `autounattend.xml` ou `unattend.xml`, é um método oficial para realizar modificações em instalações de Windows, mais detalhes podem ser encontrados na [página do Microsoft Learn](#página-do-microsoft-learn-sobre-arquivos-de-resposta) referente ao tópico. Estarei utilizando o [Schneegans autounattend.xml generator](#página-do-schneegans-autounattendxml-generator) para gerar esse arquivo.

> [!WARNING]
> Se você planeja instalar **ambos os sistemas** na mesma **unidade de armazenamento**, escolha uma das alternativas do [Schneegans autounattend.xml generator](#página-do-schneegans-autounattendxml-generator) para configurar um tamanho maior para a partição de sistema (EFI). Mais informações sobre no seguinte tópico da Arch Wiki:
> * [A partição EFI de sistema criada pelo Windows é pequena demais](./README.md#página-da-arch-wiki-sobre-partição-efi-pequena-demais)

> [!CAUTION]  
> Em um ambiente de *dual boot* certas medidas de segurança são necessárias. Confira os seguintes tópicos da Arch Wiki para mais informações:
> * [Inicialização rápida e hibernação](./README.md#página-da-arch-wiki-sobre-inicialização-rápida-e-hibernação)
> * [Hibernação e sistemas multiboot](./README.md#página-da-arch-wiki-sobre-hibernação-e-sistemas-multi-boot)
>
> **SEM AS MEDIDAS CORRETAS, HÁ RISCO DE CORRUPÇÃO DO SISTEMA**.

Após configurar, revise as opções escolhidas garantindo que todas as configurações indispensáveis foram configuradas corretamente, baixe o arquivo e salve em local seguro, em seguida faça uma cópia para o diretório raiz da mídia de instalação.

Com isso todos os passos da pré-instalação foram cobertos, continue a leitura no próximo tópico, [Instalação do Windows 11](../1-installation/README.md).

## Referências
#### Página de download do Windows 11
https://www.microsoft.com/pt-br/software-download/windows11
#### Página do Rufus
https://rufus.ie/pt_BR/
#### Página do WoeUSB
https://woeusb.github.io/WoeUSB/
#### Página do Microsoft learn sobre arquivos de resposta
https://learn.microsoft.com/pt-br/windows-hardware/manufacture/desktop/update-windows-settings-and-scripts-create-your-own-answer-file-sxs?view=windows-11
#### Página do Schneegans autounattend.xml generator
https://schneegans.de/windows/unattend-generator/
#### Página da Arch Wiki sobre partição EFI pequena demais
https://wiki.archlinux.org/title/Dual_boot_with_Windows#The_EFI_system_partition_created_by_Windows_Setup_is_too_small
#### Página da Arch Wiki sobre inicialização rápida e hibernação
https://wiki.archlinux.org/title/Dual_boot_with_Windows#Fast_Startup_and_hibernation
#### Página da Arch Wiki sobre hibernação e sistemas multi boot
https://wiki.archlinux.org/title/EFI_system_partition#Hibernation_and_multi_boot_systems