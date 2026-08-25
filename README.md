# LicenciaturasUAMI
AR app de la Lic en Ing Química UAMI

https://youtube.com/playlist?list=PLgzQ6IPRJECcmSXNISukby2RlXLKAuBHf&si=Tdzhh2nvqyoQmCcl

*** El paquete o SDK de Vuforia falta, es necesario agregarlo manualmente desde el editor de Unity.

*** Es necesario agregar el modelo 3D a la carpeta Assets manualmente. En este repositorio no se encuentra ninguno.

## Requerimientos:

- Equipo de cómputo: Windows 10/11 o macOS 10.14+, con un procesador Intel Core i5 o superior y 8GB de RAM.
- Dispositivo móvil: Android 7.0 (Nougat) o iOS 11.0 o superior.

## Configuración

1. API Compatibility Level → .NET 4.X o .NET Framework.
2. Target Architecture → ARMv7 y ARM64 (si presenta errores, desactivar ARMv7).
3. ...
4. ...

![image]()

### Versiones

La versión de AR Foundation y ARCore que aparecerá en el Package Manager dependerá de la versión de Unity que estén usando. Elijan la que aparezca.

| Editor Version | AR Foundation Version |
|----------------|-----------------------|
| 2022.3+        | 5.1                   |
| 2021.3+        | 5.1                   |

## Unity

- Unity 2021.3
- Unity 2022.1
- Unity 2022.3

Es importante que la versión de Unity que vayan a usar tenga los módulos de Android instalados. ¿Cómo saber si tienes los módulos de Android? 

1. Abre Unity Hub.
2. Ve a Installs.
3. Haz clic en el ícono ⚙️ de la versión.
4. Selecciona Add Modules.
5. Debes tener instalados:

- OpenJDK
- Android SDK & NDK Tools

Si no los tienen instalados, simplemente selecciónalos e instala.

<img width="974" height="695" alt="1" src="https://github.com/user-attachments/assets/61b93bcd-8578-413b-ad7e-c8cb8a7f4ea1" />

<img width="1198" height="831" alt="2" src="https://github.com/user-attachments/assets/b456e6ca-6adf-457b-943c-bcbdd5b067a9" />

6. Abre Unity Hub-> Crea un proyecto nuevo en 3D

<img width="2045" height="1200" alt="5" src="https://github.com/user-attachments/assets/79fc609b-6722-4498-a985-c04d55c9466b" />

## Visual Studio
Aunque no es obligatorio, se recomienda usarlo para acceder al script rápidamente.
Puedes utilizar:

- Visual Studio Community 2019
- Visual Studio Community 2022

Visual Studio debe estar correctamente instalado y configurado, y debe estar enlazado con Unity. Para hacerlo:

1. Abre el instalador de Visual Studio.
2. Selecciona la versión de Visual Studio y haz clic en Modify.
3. Añade Game Development with Unity.

4. En el proyecto de Unity en el que vayas a trabajar, ve a Edit → Preferences → External Tools → External Script Editor y selecciona la versión de Visual Studio que vas a usar.

<img width="622" height="391" alt="14" src="https://github.com/user-attachments/assets/e52cb8d4-8e39-4143-b8bd-83125d4708f6" />

## Vuforia en Unity

https://developer.vuforia.com/library/vuforia-engine/getting-started/development-environments/getting-started-vuforia-engine-unity/

- Ve a la página de descargas de Vuforia y descarga el SDK para Unity

<img width="701" height="391" alt="17" src="https://github.com/user-attachments/assets/dcf46b8f-ad67-458b-a0c3-1340f92d42be" />

- En la pestanha "Planes y Licencias" elige el plan básico, genera una licencia para el mismo
<img width="612" height="255" alt="19" src="https://github.com/user-attachments/assets/70b5cfe6-535a-468a-a314-5f33232e0b78" />

<img width="435" height="303" alt="20" src="https://github.com/user-attachments/assets/877614e0-f059-4f1f-b1f6-e82ff8761270" />

## Multiple Image Target

### Crear base de datos en Vuforia

1.  Ve a la página de administración de Vuforia y crea una nueva base de datos de seguimiento de imágenes
3.  Agrega la imagen que deseas utilizar como objeto de seguimiento y espera a que se procese.
   <img width="390" height="288" alt="18" src="https://github.com/user-attachments/assets/03ccd0ba-ddb4-46fa-bd98-a710bde29d78" />
   
5.  Descarga el archivo de licencia de Vuforia y colócalo en la carpeta de Assets en tu proyecto de Unity.
   
<img width="802" height="761" alt="3" src="https://github.com/user-attachments/assets/8d05ef2e-d1c2-41bf-b150-04429d2b1e7c" />

<img width="660" height="359" alt="21" src="https://github.com/user-attachments/assets/ef80a28e-1b4b-4b22-a4aa-1aa077198e62" />

5.  Importa el paquete de Vuforia en tu proyecto de Unity.

<img width="544" height="968" alt="6" src="https://github.com/user-attachments/assets/9344e151-4853-4b7b-b4ba-1469e0fbb1fc" />

<img width="827" height="402" alt="7" src="https://github.com/user-attachments/assets/8f05d6c1-467e-4c5b-a782-56ac7e5b9da4" />

### Importar base de datos en Unity

- Arrastra y suelta la imagen que agregaste en el paso 2 en la escena de Unity.
- Selecciona la imagen en la jerarquía y, en el inspector, cambia su configuración de imagen a «Base de datos» y selecciona la base de datos de seguimiento que creaste en el paso 1.
- Agrega una cámara a la escena y asegúrate de que esté orientada hacia la imagen de seguimiento.


### Añadir modelo para AR

Por defecto, el modelo 3D es bastante grande, así que necesitamos reducir su tamaño.

- Haz clic en el objeto de destino del modelo en el panel izquierdo y actualiza su escala en el panel derecho. Una escala X, Y y Z de 0,5 debería funcionar bien.

Tras reducir su tamaño, debería verse algo así:

- En esta etapa, debemos comprobar que nuestra configuración funciona correctamente antes de empezar a añadir nuestros propios recursos. Para iniciar el proyecto, haz clic en el botón de reproducción que se encuentra en la parte superior de la ventana.

- Si todo está configurado correctamente, debería aparecer un modelo 3D al apuntar la imagen de referencia (cubo) a la cámara del portátil.

- Puedes imprimir la imagen de referencia y armar con el archivo adjunto (pdf).

- Para detener la ejecución del proyecto, haz clic de nuevo en el botón de reproducción.

- Para cambiar el objeto 3D que se muestra, arrastra y suelta tu modelo 3D en la carpeta "Modelos" dentro de la pestaña "Proyecto" en la parte inferior izquierda de la ventana de Unity.

- Luego, arrastra ese modelo dentro de la carpeta "Model target" en el panel de jerarquía. Tu nuevo modelo debería aparecer en la ventana de escena.

## Diseño de interfaz o menú

![image]()

## Compilar y ejecutar
Asegúrate de tener conectado tu dispositivo móvil a tu computadora y que hayas habilitado la depuración USB en tu dispositivo. Luego, en Unity, ve a «File» > «Build Settings» y selecciona la plataforma de tu dispositivo móvil.

<img width="626" height="610" alt="13" src="https://github.com/user-attachments/assets/9c08a1aa-c041-47ce-9b19-2b2d05a1b43d" />

Para compilar y ejecutar la aplicación, primero debes hacer clic en «File» y luego en «Build Settings». En la ventana que aparece, asegúrate de que la plataforma seleccionada sea la de realidad aumentada que deseas utilizar.

![image](13)

Además, cambia la versión mínima de Android para que más dispositivods sean capaces de usar el apk que se va a generar.

![image](15)


A continuación, haz clic en el botón «Add Open Scenes» para agregar la escena actual al compilador. Asegúrate de que solo tengas una escena abierta antes de compilar.
![image](14)

Luego, haz clic en el botón «Build and Run» y selecciona la ubicación donde deseas guardar el archivo ejecutable de la aplicación. Espera a que el proceso de compilación termine.

![image](16)

Una vez que el proceso de compilación se ha completado con éxito, podrás ejecutar la aplicación. Dependiendo de la plataforma de realidad virtual que hayas seleccionado, deberás seguir los pasos específicos para ejecutar la aplicación en tu dispositivo.



## DEMO


https://github.com/user-attachments/assets/c6936b24-a955-41ee-95fb-b494604b86e2



## Herramientas y enlaces importantes

- Descargar Unity Hub:
    - https://unity.com/download
- Vuforia Developer portal:
    - https://developer.vuforia.com/home
- Documentación de Vuforia:
    - https://developer.vuforia.com/library/
- Vuforia Asset store:
    - https://assetstore.unity.com/packages/templates/packs/vuforia-engine-163598
- Tutoriales de Unity:
    - https://learn.unity.com/es
- Glosario de términos:
    - https://unity.com/how-to/xr-glossary#augmented-reality-(ar)
- Manual XR de Unity
     https://docs.unity3d.com/Manual/XR.html?ampDeviceId=6ab090b2-02dd-4359-8d7d-7f25e9defe7f&ampSessionId=1771958287492&ampTimestamp=1772045060538- 



