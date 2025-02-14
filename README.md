# Detecção de pessoa utilizando celular

Este projeto utiliza a biblioteca OpenCV para detecção de objetos e faces em tempo real usando uma webcam. Ele combina o uso do modelo YOLO para detectar objetos, que nesse caso é o celular, e um classificador Haar Cascade para detectar rostos humanos. Se um rosto e o celular estiverem no vídeo ao mesmo tempo, então aquela pessoa está utilizando o celular.

## Funcionalidades

1. **Detecção de Objetos com YOLO:**
   - O modelo processa o vídeo da webcam e detecta objetos, desenhando caixas ao redor dos objetos detectados.

2. **Detecção de Faces:**
   - A detecção de rostos é feita utilizando o classificador Haar Cascade da OpenCV.

3. **Integração das Deteções:**
   - O código detecta simultaneamente objetos e rostos em cada quadro do vídeo.
   - Caso um "celular" seja detectado e um rosto também seja identificado, uma mensagem "Usando celular" é exibida no vídeo.

4. **Captura de Vídeo:**
   - O código utiliza a webcam do computador para capturar o vídeo e aplicar as detecções.

## Arquivos Necessários

- **Arquivos de Configuração e Pesos do YOLO:**
  O código carrega os arquivos de configuração (`.cfg`) e pesos (`.weights`) do modelo YOLO. Esses arquivos podem ser encontrados na [página oficial do YOLO](https://pjreddie.com/darknet/yolo/) ou podem ser baixados diretamente de fontes como o repositório do modelo YOLO.

- **Arquivo de Classes:**
  O arquivo `coco.names` contém as classes dos objetos que o modelo pode detectar objetos(no caso o celular).

## Requisitos
- Python 3.x
- OpenCV (`cv2`)
- NumPy (`numpy`)
#   i a - f i n a l  
 