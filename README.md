# Como instalar o MacOS Big Sur no VirtualBox Windows 2023

Neste guia, orientaremos você em todas as etapas para instalar o macOS Big Sur no VirtualBox Windows. Mostraremos cada etapa com capturas de tela e um vídeo para orientá-lo visualmente. Como pode haver problemas de compatibilidade do sistema com instalações como esta, confira nosso fórum. O novo fórum GEEKrar é um ótimo lugar para postar perguntas ou encontrar soluções para problemas frequentes.

## O que é macOS Big Sur

O macOS Big Sur é o 17º lançamento do sistema operacional Mac para computadores Macintosh e é o sucessor do macOS Catalina. O sistema operacional foi lançado oficialmente ao público em 12 de novembro de 2020 e está disponível para uma série de computadores Mac e também pode ser instalado virtualmente, como neste guia.

## O que você precisa para esta instalação:
- Windows10
- 8GB RAM
- 60 GB de espaço livre em disco
- VirtualBox Oracle VM VirtualBox Extension Pack ([**Baixar**](https://www.mediafire.com/file/irna8hwybkhl41f/BigSur13-3-1.iso/file))
- Arquivo de imagem ISO do MacOS Big Sur ([**Baixar**](https://www.mediafire.com/file/irna8hwybkhl41f/BigSur13-3-1.iso/file))
- Comandos no CMD como Administrador

## Criar maquina virtual
Para começar, precisamos instalar o VirtualBox Windows. Se você já fez isso, este artigo o guiará por todo o processo. Depois que o VirtualBox estiver funcionando, queremos garantir que você tenha seu arquivo de comando e o arquivo ISO do Big Sur à mão. Vamos precisar deles para prosseguir.

1.1. No Oracle VM VirtualBox Manager, como o ícone azul 'Novo' na parte superior

![Crie uma nova VM para instalar o macOS Big Sur no VirtualBox Windows](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)

1.2. Na primeira janela, estaremos nomeando e identificando o tipo de máquina virtual que estamos criando. No campo Name, digite ‘BigSur.’ O campo Machine Folder pode permanecer como padrão, a menos que você tenha um motivo para alterá-lo. O tipo será Mac OS X. A versão será ‘macOS 10.13 High Sierra (64 bits).

![Etiquetar máquina virtual](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)

1.3. Em Tamanho da memória, queremos aumentar a memória disponível para pelo menos 8 GB de RAM. Clique em Avançar

![Forneça pelo menos 8 GB de RAM ou 50% do disponível](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)

1.4. 'Disco rígido', vamos deixar o padrão 'Criar um disco rígido virtual agora' e clicar em 'Criar'.

![Disco rígido](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)

1.5. O ‘tipo de arquivo de disco rígido’ também permanecerá com o VHD (Disco Rígido Virtual) padrão. Clique em Avançar.

![Tipo de arquivo do disco rígido](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)

1.6. 'Armazenamento no disco rígido físico' será alocado dinamicamente.

![Armazenamento em disco físico](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)

1.7. Em 'Localização e tamanho do arquivo', estamos deixando o caminho da pasta padrão, mas abaixo do tamanho do disco, queremos aumentá-lo para pelo menos 60 GB. Eu tentei 40 GB e 50 GB com muitos problemas. Portanto, 60 ou mais é fortemente sugerido. Depois de concluído, clique em 'Criar' e conclua a primeira etapa.

![65 GB é o espaço mínimo recomendado](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)

## Modificar o VirtualBox com CMD

Agora que o novo VirtualBox foi criado, precisamos executar alguns comandos para modificá-lo e continuar executando o macOS Big Sur. Se você não baixou o texto do arquivo de comando, clique aqui para obtê-lo.

2.1. Abra o arquivo de texto, vá para o menu 'Editar' na parte superior e depois para baixo até 'Substituir ..." Aqui, queremos digitar "VBoxNAME" no campo 'Localizar'. No campo 'Substituir por', digite o nome que você chamou de VirtualBox (etapa 2). Clique no botão 'Substituir tudo', e isso deve converter todos os itens com o novo nome de arquivo.

![Antes da substituição do VBoxNAME](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)

![Após a substituição](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)

2.2. Agora vá até o prompt de comando (Iniciar, digite 'cmd' e aperte enter), cole a primeira linha e aperte enter. (execute o prompt de comando como administrador)

cd "C:\Arquivos de Programas\Oracle\VirtualBox\"

2.3. Este comando nos deslocará para o diretório Windows do VirtualBox e estaremos prontos para os próximos comandos.

![Diretório do Windows VirtualBox](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)

2.4. Antes de prosseguir, verifique se você está no diretório acima. Se você não estiver lá, você deve navegar para lá agora antes de prosseguir.

Realce e copie as próximas seis linhas, cole-as na janela de comando e pressione enter.

![copiar comandos](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)

2.5. Feito isso, podemos fechar todas as janelas e começar a carregar o macOS Big Sur no VirtualBox Windows.
