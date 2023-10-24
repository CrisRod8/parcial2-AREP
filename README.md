# parcial2-AREP

Autor: Cristian Fernando Rodríguez González  

## EJECUCIÓN LOCAL
1. Clonar el repositorio usando el código a continuación:  
    ```
    git clone https://github.com/CrisRod8/parcial2-AREP.git
    ```

2. Dentro de la carpeta creada abrimos el cmd y ejecutamos el siguiente comando:
   
   ```
   mvn clean install
   ```

3. Para probarlo localmente, ejecutamos:

   ```
   java -cp "target/classes;target/dependency/*" org.example.Main
   ```

4. Ahora podemos entrar en cualquier browser con: http://localhost:4567/collatzsequence

## EJECUCIÓN DOCKER  

1. Crear Dockerfile.
2. Ejecutar para crear la imagen:
   ```
   docker build --tag parcial .
   ```
3. Crear contenedor:
   ```
   docker run -d -p 34000:6000 --name contenedor parcial
   ```
4. Probamos: http://localhost:34000/collatzsequence

## AWS  
1. Se lanza una instancia de EC2.
2. Se configura el puerto en grupos de seguridad.
3. Se conecta a la instancia, al hacer la conexión se instala docker y se hace pull de la imagen creada y respectivamente subida a Docker Hub:
   ![image](https://github.com/CrisRod8/parcial2-AREP/assets/111186898/0c38d144-5ea2-4ce7-af64-3cbfde827a5e)
4. Finalmente podemos entrar al un link como: http://ec2-54-166-246-32.compute-1.amazonaws.com:35000/collatzsequence y ver:
   ![image](https://github.com/CrisRod8/parcial2-AREP/assets/111186898/b40c7c39-1fe2-4946-a370-0a5180d4f23e)

## VIDEO  

https://www.youtube.com/shorts/msRE6vfEe_Y


 
   


   

   
