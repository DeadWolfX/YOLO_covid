##############################################################Resultados de entrenamiento de Yolov5s###########################################################################
Aquí se encuentran los resultados del entrenamiento de la arquitectura yolov5s proporcionada en https://github.com/ultralytics/yolov5 

Se entreno por 149 epocas donde se paro por el metodo de early stop en la epoca 48 se guarda la ultima y la de mejor desempeño
Se entreno usando los datos de rsna pneumonia  incluyendo recuadros delimitadores de 0x0 pixel para los que no tenian detección, se ordenaron por clases [c1,c2] y se distribuyeron equitativamente para los data sets
es decir train=0.8c1+0.8c2 validation=0.1c1+0.1c2 test=0.1c1+0.1c2 para que las calses esten menos sobrerepresentadas en cada dataset
