##############################################################Resultados de entrenamiento de Yolov5s###########################################################################
Aquí se encuentran los resultados del entrenamiento de la arquitectura yolov5s proporcionada en https://github.com/ultralytics/yolov5 

Se entreno por 220 epocas donde se paro por el metodo de early stop en la epoca 119 se guarda la ultima y la de mejor desempeño
Se entreno usando los datos de simm-covid  incluyendo recuadros delimitadores de 0x0 pixel para los que no tenian detección, se ordenaron por clases [c1,c2,c3,c4] y se distribuyeron equitativamente para los data sets
es decir train=0.8c1+0.8c2+0.8c3+0.8ca validation=0.1c1+0.1c2+0.1c3+0.1ca =0.1c1+0.1c2+0.1c3+0.1ca para que las calses esten menos sobrerepresentadas en cada dataset
