# Reconhecimento Facial e transformação de imagens em Dados no Azure ML

### Documentação criada para mostrar como realizar a detecção de rostos, extração de textos de imagens, geração de legenda, criação de tags e detecção de objetos utilizando o Azure Vision Studio.

> [!Important]
> Num navegador web, navegue até **Vision Studio** em **https://portal.vision.cognitive.azure.com** para explorar todas as opções.

## Detecte rostos no Vision Studio

1. Na página inicial **Getting started with Vision**, selecione a guia **Face** e, em seguida, selecione o bloco **Detect Faces in an image**.
   
1. No subtítulo **Try It Out**, reconheça a política de uso de recursos lendo e marcando a caixa.

1. Selecione cada uma das imagens de amostra e observe os dados de detecção facial retornados.

![image](https://github.com/dani-peixoto/lab-vision-studio/assets/3649843/11a7a65d-b5ed-4a5d-b0f3-8282568a0e48)

## Extraia texto de imagens no Vision Studio

1. Na página inicial **Getting started with Vision**, selecione **Optical character recognition** e, em seguida, o bloco **Extract text from images**.

1. No subtítulo **Try It Out**, reconheça a política de uso de recursos lendo e marcando a caixa.

1. Selecione cada uma das imagens de amostra e revise o que é retornado.
   
   - Nos atributos detectados , qualquer texto encontrado na imagem é organizado em uma estrutura hierárquica de regiões, linhas e palavras.
   - Na imagem, a localização do texto é indicada por uma caixa delimitadora, conforme mostrado aqui:
  
![image](https://github.com/dani-peixoto/lab-vision-studio/assets/3649843/79a3d8ad-f3ad-4717-9803-8e0d0e1206fd)

## Gerar legendas para uma imagem

💡 Vejamos a funcionalidade de legenda de imagens do Azure AI Vision. As legendas das imagens estão disponíveis por meio dos recursos **Caption** e **Denses captions**.

1. Na página inicial **Getting started with Vision**, selecione **Image analysis** e, em seguida, o bloco **Add captions to images**.
   
1. No subtítulo **Try It Out**, reconheça a política de uso de recursos lendo e marcando a caixa.
   
1. Observe o texto da legenda gerado, visível no painel Atributos detectados à direita da imagem.

1. A funcionalidade Caption fornece uma única frase em inglês legível que descreve o conteúdo da imagem.

![image](https://github.com/dani-peixoto/lab-vision-studio/assets/3649843/549f3891-b77e-4488-b47a-b4f307fb9a6a)

5. Em seguida, use a mesma imagem para realizar legendas densas. Retorne à página inicial do Vision Studio e, como fez antes, selecione a guia **Image analysis** e, em seguida, selecione o bloco **dense captions**.

![image](https://github.com/dani-peixoto/lab-vision-studio/assets/3649843/b24b5c5a-6f5c-471b-b343-96c44dd81e5d)

📣 O recurso Dense Captions difere do recurso Caption porque fornece diversas legendas legíveis para uma imagem, uma descrevendo o conteúdo da imagem e outras, cada uma cobrindo os objetos essenciais detectados na imagem. Cada objeto detectado inclui uma caixa delimitadora, que define as coordenadas dos pixels na imagem associada ao objeto.

## Marcando imagens

💡 O próximo recurso que você experimentará é a funcionalidade Extrair Tags. Extrair tags é baseado em milhares de objetos reconhecíveis, incluindo seres vivos, cenários e ações.

1. Na página inicial **Getting started with Vision**, selecione **Extract common tags from images** e, em seguida, o bloco **Image analysis tab**.

1. Em Escolha o modelo que deseja experimentar, deixe selecionado **Prebuilt product vs. gap model**. Em Escolha seu idioma, selecione English ou um idioma de sua preferência.

1. Selecione cada uma das imagens de amostra e observe as tags retornadas.

![image](https://github.com/dani-peixoto/lab-vision-studio/assets/3649843/42f1f39b-bca8-4be6-adc6-bb901af448ad)

## Detecção de objetos

💡 A detecção de objetos detecta e extrai caixas delimitadoras com base em milhares de objetos e seres vivos reconhecíveis.

1. Na página inicial **Getting started with Vision**, selecione **Detect common objects in images** e, em seguida, o bloco **Image analysis tab**.

1. Em Escolha o modelo que deseja experimentar, deixe selecionado **Prebuilt product vs. gap model**.

1. Na caixa Atributos detectados , observe a lista de objetos detectados e suas pontuações de confiança.

1. Passe o cursor do mouse sobre os objetos na lista Atributos detectados para destacar a caixa delimitadora do objeto na imagem.

1. Mova o controle deslizante Valor limite até que um valor de 70 seja exibido à direita do controle deslizante. Observe o que acontece com os objetos da lista. O controle deslizante de limite especifica que somente objetos identificados com uma pontuação de confiança ou probabilidade maior que o limite devem ser exibidos.

![image](https://github.com/dani-peixoto/lab-vision-studio/assets/3649843/f01d81a5-dedd-423f-ab21-021e2d686aea)
