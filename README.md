# Taller Azure Remote Rendering

A continuación se muestran los pasos para utilizar esta herramienta en Unity.

## Requerimientos
- [Visual Studio Community 2019](https://visualstudio.microsoft.com/es/vs/older-downloads/)
  - Desarrollo de la plataforma universal de Windows
  - Desarrollo para escritorio con C++
  - Desarrollo con juego en Unity
- [Unity Hub](https://unity.com/es/download)
  - Unity 2020.3.X
- [Windows SDK](https://developer.microsoft.com/en-us/windows/downloads/windows-sdk/?wt.mc_id=studentamb_159817)
- [HoloLens 2 Emulator](https://learn.microsoft.com/en-us/windows/mixed-reality/develop/advanced-concepts/hololens-emulator-archive?wt.mc_id=studentamb_159817)
- [Git](https://git-scm.com/downloads)
- [GitHub Desktop](https://desktop.github.com/) (*Opcional*)
- Una cuenta de Azure
  - [Cuenta gratuita](https://azure.microsoft.com/es-es/free/?wt.mc_id=studentamb_159817)
  - [Cuenta educativa](https://azure.microsoft.com/es-es/free/students/?wt.mc_id=studentamb_159817)
  
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
1. Abrir el proyecto, con la opción *add proyect from disk*, que se encuentra en **azure-remote-rendering/Unity/Quickstart**. Actualice o instale la versión de Unity si es necesario.
2. Configurar para que utilice la plataforma universal de Windows. **File -> Build Settings -> Universal Windows Platform -> Switch Platform**
3. Abrir la escena **Quickstart**: el archivo **assets/Scenes/Quickstart**
4. En **Hierarchy** seleccionar **Remote Rendering**
5. En **Inspector**, en el componente **Remote Rendering** capturar el id del recurso en Azure, así como el dominio y la clave.
6. Ejecutar el programa
7. Para mover la cámara o el objeto utilice las herramientas *move* y *rotate* dentro de la escena.

## Recursos
- [Introducción a Azure Remote Rendering](https://learn.microsoft.com/es-es/training/modules/intro-to-azure-remote-rendering/?wt.mc_id=studentamb_159817)
- [Representación de un modelo con Azure Remote Rendering](https://learn.microsoft.com/es-es/training/modules/render-model-azure-remote-rendering-unity/?wt.mc_id=studentamb_159817)
- [Configuración de un proyecto de realidad mixta en Unity con el kit de herramientas de Mixed Reality](https://learn.microsoft.com/es-es/training/modules/mixed-reality-toolkit-project-unity/?wt.mc_id=studentamb_159817)
