# Dual Boot - Arch Linux | Windows 11

## Introdução

Este repositório documenta minha configuração de *dual boot* entre **Arch Linux** e **Windows 11**, incluindo referências, ferramentas, softwares e repositórios utilizados. Sinta-se à vontade para usar este material como base para criar sua própria documentação sobre o processo.

## Público alvo

Este material é destinado a usuários que desejam realizar ou compreender o processo de *dual boot* entre **Windows 11** e **Arch Linux**. O conteúdo pressupõe que o leitor possua conhecimentos básicos sobre:  

**Informática e sistemas operacionais**: Familiaridade com a interface do sistema, instalação de software e gerenciamento de arquivos.  
**Arquitetura de computadores**: Compreensão dos componentes principais, como CPU, RAM e armazenamento, e como eles interagem.  
**Ambientes de linha de comando**: Conforto em executar comandos e navegar por interfaces baseadas em texto.  
**Seguir instruções técnicas e pesquisar dúvidas**: Habilidade para interpretar guias e buscar informações adicionais quando necessário.


## Estrutura de arquivos

Os registros estão divididos em 2 diretórios principais `\win11` e `\arch`, contendo os conteúdos relacionados ao respectivo sistema operacional. Os tópicos de cada diretório estão divididos em 3 subdiretórios `\0-pre-install`, `\1-installation`, `\2-post-install`, cobrindo respectivamente os processos de pré-instalação, instalação e pós-instalação.

A navegação entre arquivos conta com o auxílio de um sumário em todos os arquivos `README.md` como o seguinte:

**Sumário**

* [Introdução](./README.md#introdução): Introdução do projeto.
* [Público alvo](./README.md#público-alvo): Descrição do público alvo e conhecimentos nescessários.
* [Estrutura de arquivos](./README.md#estrutura-de-arquivos): Detalhes da estrutura de arquivos.
* [Licença](./README.md#licença): Sobre a licença do repositório.
* [Atualizações](./README.md#atualizações): Instruções para acompanhar atualizações.
* [Referências](./README.md#referências): Lista de referências utilizadas.

[Windows 11](./win11/README.md)
* [Pré-instalação](./win11/0-pre-install/README.md): Preparo da mídia de instalação do Windows 11, configuração do arquivo `autounattend.xml`.
* [Instalação](./win11/1-installation/README.md): Instalação do Windows 11 considerando as etapas realizadas na pré-instalação.
* [Pós-instalação](./win11/2-post-install/README.md): Configurações de sistema, instalação e configuração de softwares.

[Arch Linux](./arch/README.md)  
* [Pré-instalação](./arch/0-pre-install/README.md): Recomendações gerais, preparo da mídia de instalação do Arch Linux.
* [Instalação](./arch/1-installation/README.md): Instalação do Arch Linux considerando as etapas realizadas na pré-instalação.
* [Pós-instalação](./arch/2-post-install/README.md): Configurações de sistema, instalação e configuração de softwares.

## Licença

Este repositório está sob os termos da licença `Attribution-NonCommercial-ShareAlike 4.0 International`. Para mais detalhes, acesse a [licença](./LICENSE).

## Atualizações

As atualizações deste repositório podem ser acompanhadas diretamente no *GitHub*. Recomendo verificar periodicamente para novas informações ou melhorias.

## Referências

Recursos e referências serão adicionados pontualmente durante a escrita do projeto.