# LicenciaturasUAMI
AR app de la Lic en Ing Química UAMI

*** El paquete o SDK de Vuforia falta, es necesario agregarlo manualmente desde el editor de Unity.

*** Es necesario agregar el modelo 3D a la carpeta Assets manualmente. En este repositorio no se encuentra ninguno.

## Requerimientos:
### Unity

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

### Visual Studio
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

### Configuración

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


## Diseño de interfaz o menú

![image]()

## Vuforia en Unity

### Multiple Image Target

### Crear base de datos en Vuforia

### Importar base de datos en Unity

### Crear el botón virtual

### Diseñar el botón

### Añadir modelo para AR

### Script Button Manager

### Agregar y referenciar Button Manager

## DEMO




