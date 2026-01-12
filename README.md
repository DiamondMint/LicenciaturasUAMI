# LicenciaturasUAMI
AR app de la Lic en Ing Química UAMI

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

![image]()

6. Abre Unity Hub-> Crea un proyecto nuevo en 3D

## Visual Studio
Aunque no es obligatorio, se recomienda usarlo para acceder al script rápidamente.
Puedes utilizar:

- Visual Studio Community 2019
- Visual Studio Community 2022

Visual Studio debe estar correctamente instalado y configurado, y debe estar enlazado con Unity. Para hacerlo:

1. Abre el instalador de Visual Studio.
2. Selecciona la versión de Visual Studio y haz clic en Modify.
3. Añade Game Development with Unity.

![image]()

4. En el proyecto de Unity en el que vayas a trabajar, ve a Edit → Preferences → External Tools → External Script Editor y selecciona la versión de Visual Studio que vas a usar.

![image]()


## Vuforia en Unity

### Multiple Image Target

### Crear base de datos en Vuforia

1.  Ve a la página de administración de Vuforia y crea una nueva base de datos de seguimiento de imágenes
2.  Agrega la imagen que deseas utilizar como objeto de seguimiento y espera a que se procese.
3.  Descarga el archivo de licencia de Vuforia y colócalo en la carpeta de Assets en tu proyecto de Unity.
![image]()
   
5.  Importa el paquete de Vuforia en tu proyecto de Unity.

### Importar base de datos en Unity

- Arrastra y suelta la imagen que agregaste en el paso 2 en la escena de Unity.
- Selecciona la imagen en la jerarquía y, en el inspector, cambia su configuración de imagen a «Base de datos» y selecciona la base de datos de seguimiento que creaste en el paso 1.
- Agrega una cámara a la escena y asegúrate de que esté orientada hacia la imagen de seguimiento.


### Crear el botón virtual

### Diseñar el botón

### Añadir modelo para AR

### Script Button Manager

### Agregar y referenciar Button Manager

## Diseño de interfaz o menú

![image]()

## Compilar y ejecutar
Asegúrate de tener conectado tu dispositivo móvil a tu computadora y que hayas habilitado la depuración USB en tu dispositivo. Luego, en Unity, ve a «File» > «Build Settings» y selecciona la plataforma de tu dispositivo móvil.

Para compilar y ejecutar la aplicación, primero debes hacer clic en «File» y luego en «Build Settings». En la ventana que aparece, asegúrate de que la plataforma seleccionada sea la de realidad virtual que deseas utilizar.

![image](13)

Además, cambia la versión mínima de Android para que más dispositivods sean capaces de usar el apk que se va a generar.

![image](15)


A continuación, haz clic en el botón «Add Open Scenes» para agregar la escena actual al compilador. Asegúrate de que solo tengas una escena abierta antes de compilar.
![image](14)

Luego, haz clic en el botón «Build and Run» y selecciona la ubicación donde deseas guardar el archivo ejecutable de la aplicación. Espera a que el proceso de compilación termine.

![image](16)

Una vez que el proceso de compilación se ha completado con éxito, podrás ejecutar la aplicación. Dependiendo de la plataforma de realidad virtual que hayas seleccionado, deberás seguir los pasos específicos para ejecutar la aplicación en tu dispositivo.



## DEMO

## Herramientas y enlaces importantes

- Descargar Unity Hub:
    - https://unity.com/download
- Vuforia Developer portal:
    - https://developer.vuforia.com/home
- Documentación de Vuforia:
    - https://developer.vuforia.com/library/
- Tutoriales de Unity:
    - https://learn.unity.com/es
- Asset store:
    - https://assetstore.unity.com/packages/templates/packs/vuforia-engine-163598




