FROM python:3.8

WORKDIR /app

# el primer parametro(lado de la derecha) es el de mi entorno local
# y el lado de la izquierda es el lado del contenedor
# El comando tambien pudo haber sido escrito de la siguiente forma:
#   COPY requirements.txt requirements.txt
COPY requirements.txt /app/requirements.txt


# el flag upgrade  no afecta las dependencias, solo mira si hay
# actualizaciones en el gestor de paquetes 
RUN pip install --no-cache-dir --upgrade -r /app/requirements.txt

COPY . /app/

#este comando es el que mantendra encendido el contenedor
CMD bash -c "while true; do sleep 1; done"

