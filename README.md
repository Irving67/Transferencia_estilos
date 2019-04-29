# Transferencia_estilos
Proyecto de redes neuronales preentrenadas dedicado a la transferencia de estilos entre imágenes

El siguiente proyecto tiene como objetivo la implementación de una red neuronal preentrenada (mnist) para realizar la combinación de una imagen base con el estilo encontrado en otra imagen, para ello se emplea el uso de keras y tensroflow, las cuales se describe como instalar a continuación (El proyecto se realizó originalmente para el sistema operativo Ubuntu 16.04 y por medio del ambiente de Jupyter, instalado junto con Keras y Tensroflow):

Pasos a seguir para instalación en Ubuntu 16.04:

Instalar el ambiente 
1. Descargar e Instalar miniconda para 64bits y para python3.6  https://conda.io/miniconda.html, mediante bash Miniconda3-latest-Linux-x86_64.sh (Decir siempre “yes”)
Cerrar y abrir una nueva ventana
2. Instalar el ambiente virtual conda env create -f user -cpu.yml
3. Limpiar archivos descargados conda clean -tp
4. Probar instalación ejecutando el programa mnist.ipynb en la terminal para ver si se ejecuto completemente. 
source activate actumlogos-cpu
jupyter notebook NeuralStyleTransfer.ipynb  


Pasos a seguir para uso en windows u otros sistemas:

Instalar Anaconda Navigator
1. Descargar e Instalar Anaconda Navigator para 64bits y para el sistema operativo correspondiente en el siguiente enlace:  https://anaconda.org/anaconda/anaconda-navigator.
2. Seguir pasos de instalación del del mismo instalador
3. Una vez teniendo el ambiente instalado, en el navegador ir a la sección de "Enviroment" y en la sección de paquetes seleccionar "Not Installed", para buscar el paquete de Keras (Deep Learning Library for theano and tensorflow)
4.- Seleccionar Aplly y esperar la instalación
5.- Iniciar un Nootebook de Jupyter en la sección Home y seleccionar el archivo NeuralStyleTransfer.ipynb 
6.- Probar funcionamiento del programa




















Instructivo de instalación para usar GPUs

4.	Instalar Ubuntu 16.04 (con conexión a internet para que instala el driver para la tarjeta Nvidia) 

5.	Instalar el sorporte para usar GPUs (instrucciones completas en https://www.tensorflow.org/install/install_linux)
•	Instalar CUDA® Toolkit 8.0 siguiendo las instrucciones en  http://docs.nvidia.com/cuda/cuda-installation-guide-linux/#axzz4VZnqTJ2A
•	Instalar cuDNN v5.1 seguir las instrucciones en https://developer.nvidia.com/cudnn 
•	Instalar la librería libcupti-dev mediante 
sudo apt-get install libcupti-dev
•	Añadir al bashrc  
export CUDA_HOME=/usr/local/cuda-8.0
export LD_LIBRARY_PATH=${CUDA_HOME}/lib64:$LD_LIBRARY_PATH
export PATH=${CUDA_HOME}/bin:${PATH}
Instrucciones completas en http://www.pyimagesearch.com/2016/07/04/how-to-install-cuda-toolkit-and-cudnn-for-deep-learning/ 

6.	Instalar el ambiente 
•	Descargar e Instalar miniconda https://conda.io/docs/install/quick.html#linux-miniconda-install, mediante 
bash Miniconda3-latest-Linux-x86_64.sh
Decir siempre “yes”
Cerrar y abrir una nueva ventana
•	Instalar el ambiente virtual 
conda env create -f actumlogos-gpu.yml
•	Limpiar archivos descargados  
conda clean -tp

7.	Probar instalación ejecutando el programa mnist.py en la terminal para ver si se ejecuto completemente. 
source activate actumlogos-gpu
jupyter notebook mnist.ipynb  
