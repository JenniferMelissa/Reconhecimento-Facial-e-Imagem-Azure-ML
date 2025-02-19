
<h1 align="center"> Reconhecimento Facial e Imagem Azure ML</h1>

## Primeiro Passo: Criar um recurso de serviços de IA do Azure 

Você pode usar os recursos de OCR do Azure AI Vision com um recurso multisserviço de serviços do Azure AI . Se você ainda não fez isso, crie um recurso de serviços do Azure AI na sua assinatura do Azure.

1 - Em outra aba do navegador, abra o portal do Azure em https://portal.azure.com, entrando com a conta da Microsoft associada à sua assinatura do Azure.

2 - Clique no botão ＋ Criar um recurso e pesquise por Azure AI services. Selecione criar um plano de serviços Azure AI . Você será levado para uma página para criar um recurso de serviços Azure AI. Configure-o com as seguintes configurações:
- Assinatura : sua assinatura do Azure.
- Grupo de recursos : selecione ou crie um grupo de recursos com um nome exclusivo.
- Região : Selecione a região geográfica mais próxima. Se estiver no leste dos EUA, use “East US 2”.
- Nome : Insira um nome exclusivo.
- Nível de preço : Padrão S0.

3 - Ao marcar esta caixa, reconheço que li e compreendi todos os termos abaixo : Selecionado.
4 - Selecione Revisar + criar e depois Criar e aguarde a conclusão da implantação.


## Segundo Passo: Conecte seu recurso de serviço de IA do Azure ao Vision Studio

1 - Em seguida, conecte o recurso de serviços de IA do Azure que você provisionou acima ao Vision Studio.

2 - Em outra aba do navegador, navegue até o Vision Studio em https://portal.vision.cognitive.azure.com.

3 - Entre com sua conta e certifique-se de estar usando o mesmo diretório onde você criou seu recurso de serviços de IA do Azure.

4 - Na página inicial do Vision Studio, selecione Exibir todos os recursos no título Introdução ao Vision.

5 - Na página Selecionar um recurso para trabalhar , passe o cursor do mouse sobre o recurso que você criou acima na lista, marque a caixa à esquerda do nome do recurso e selecione Selecionar como recurso padrão.

6 - Feche a página de configurações selecionando o “x” no canto superior direito da tela.

7 -  Deixe a caixa selecioanda onde está escrito 'I ancknowledge that this demo will incur usage to resurce in my Azure Account'.

## Exemplo 1 - Adicione legendas às imagens

1 - Em um navegador da Web, navegue até o Vision Studio em https://portal.vision.cognitive.azure.com .

2 - Na página inicial da Introdução ao Vision, no meu exemplo, selecionei a aba de 'Imagem Analysis' e escolhi a opção 'Add captions to image' onde será gerado uma frase legível que descreva o conteúdo de uma imagem..

3 - Selecionei a imagem 1.png do arquivo input, e foi gerado o seguinte resultado: 'A group os people celebrating' (Um grupo de pessoas celebrando).

<img src="output/1.PNG" alt="some text" width=500 height=500>

4 - E dessa forma, ele transcreveu o conteudo da imagem.

## Exemplo 2 - Detecção de Faces em Imagens

1 - Em um navegador da Web, navegue até o Vision Studio em https://portal.vision.cognitive.azure.com .

2 - Na página inicial da Introdução ao Vision, no meu exemplo, selecionei a aba de 'Face' e escolhi a opção 'Detect faces in an image', onde ira detectar a localização de um ou mais rostos humanos em imagens, juntamente com atributos como pose, máscara facial e pontos de referência faciais.

3- Selecionei a imagem 2.png do arquivo input, fiz a detecção, trazendo o resultado abaixo: 

<img src="output/2.PNG" alt="some text" width=500 height=500>

4 - Dessa forma, ele fez a leitura e trouxe a quantidade de faces da minha imagem.


## Exemplo 3 - Extraindo texto de Imagens

1 - Em um navegador da Web, navegue até o Vision Studio em https://portal.vision.cognitive.azure.com .

2 - Na página inicial da Introdução ao Vision, no meu exemplo, selecionei a aba de 'Face' e escolhi a opção 'Optical character recognition', onde é usado uma API Read para extrair texto impresso e manuscrito em idiomas suportados de imagens, PDFs e arquivos TIFF. O recurso de reconhecimento óptico de caracteres (OCR) oferece suporte a imagens e documentos com idiomas mistos e não exige a especificação do idioma.

3- Selecionei a imagem 3.png do arquivo input, para que seja transcrito o texto da imagem, onde trouxe o resultado abaixo: 

vitórial
àsuaverdadeira
queoconduzirá
éocaminho
prin
queesse
vocêentenderá
devontade,
força
quandohá
ouincertezas,
265
nascertezas
265
ounabravura,
610
nomedo
ounatristeza,
naglória
ounaconquista,
6
naderrota
batalha,
Acada

<img src="output/3.PNG" alt="some text" width=500 height=500>

Vale resaltar, que a IA conseguiu transcrever corretamente todas as palavras da imagem, e ainda adicionou alguns valores que para ele fazem sentido.


