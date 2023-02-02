# Taller Azure Remote Rendering

A continuación se muestran los pasos para utilizar esta herramienta en Unity.

## Requerimientos
- [Visual Studio Community 2019](https://visualstudio.microsoft.com/es/vs/older-downloads/)
  - Desarrollo de la plataforma universal de Windows
  - Desarrollo para escritorio con C++
  - Desarrollo con juego en Unity
- [Unity Hub](https://unity.com/es/download)
  - Unity 2020.3.X
- [Windows SDK](https://developer.microsoft.com/en-us/windows/downloads/windows-sdk/)
- [HoloLens 2 Emulator](https://learn.microsoft.com/en-us/windows/mixed-reality/develop/advanced-concepts/hololens-emulator-archive)
- [Git](https://git-scm.com/downloads)
- [GitHub Desktop](https://desktop.github.com/) (*Opcional*)
- Una cuenta de Azure
  - [Cuenta gratuita](https://azure.microsoft.com/es-es/free/)
  - [Cuenta educativa](https://azure.microsoft.com/es-es/free/students/)
  
## Portal de Azure
1. Accede al portal de Azure
2. Crea un servicio de Azure Remote Rendering
    1. Asigna un nombre
    2. Selecciona una región
    3. Asigna un grupo de recursos
3. Guardar el id del recurso, el dominio y la clave 
  
## Proyecto de inicio rápido
  
1. Clonar el repositorio de Azure Remote Rendering: [https://github.com/Azure/azure-remote-rendering](https://github.com/Azure/azure-remote-rendering)
2. Abrir la consola en el directorio donde se encuentra la carpeta ```azure-remote-rendering```
3. Ejecutar el siguiente comando: 
```
powershell -ExecutionPolicy RemoteSigned -File azure-remote-rendering\Scripts\DownloadUnityPackages.ps1
```
  
## Unity Hub
1. Abrir el proyecto que se encuentra en **azure-remote-rendering/Unity/Quickstart**
2. Configurar para que utilice la plataforma universal de Windows
3. Abrir el archivo **assets/Scenes/Quickstart**
4. En **Hierarchy** seleccionar **Remote Rendering**
5. Capturar el id del recurso en Azure, así como el dominio y la clave
6. Ejecutar el programa

## Recursos
- [Introducción a Azure Remote Rendering](https://learn.microsoft.com/es-es/training/modules/intro-to-azure-remote-rendering/)
- [Representación de un modelo con Azure Remote Rendering](https://learn.microsoft.com/es-es/training/modules/render-model-azure-remote-rendering-unity/)
- [Configuración de un proyecto de realidad mixta en Unity con el kit de herramientas de Mixed Reality](https://learn.microsoft.com/es-es/training/modules/mixed-reality-toolkit-project-unity/)
