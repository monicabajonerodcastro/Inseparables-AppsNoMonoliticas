# Inseparables-AppsNoMonoliticas

## Prerequisitos
- Oracle Java u OpenJDK (JRE 11 o mayor)
- VisualStudio Code
- [Graphviz](https://www.graphviz.org/) instalado en el sistema.

## Instrucciones de instalación y generación del mapa de contexto.
1. Abrir el proyecto en VisualStudio Code
2. Instalar las siguientes extensiones:
    a. [Context Mapper](https://marketplace.visualstudio.com/items?itemName=contextmapper.context-mapper-vscode-extension)
    b. [PlantUML](https://marketplace.visualstudio.com/items?itemName=jebbs.plantuml)
3. Abrir cualquier archivo de la carpeta `ContextMap`: En el archivo `pda-context-mapper-as-is` encontrará la definición del dominio, subdominios, contextos y mapa de contexto de AS-IS. En el archivo `pda-context-mapper-to-be` encontrará la definición del dominio, subdominios, contextos y mapa de contexto de AS-IS. 
4. Clic derecho en cualquier parte del código del archivo y seleccionar la opción: `Generate Graphical Context Map`
5. En la parte superior se mostrará un cuadro con los diferentes formatos en los que se puede generar el mapa. Elija los que considere necesarios.
6. En la carpeta `src-gen` se encontrarán el archivo generado.

**NOTA:** Por defecto se encuentra en la carpeta los diagramas en formato `.png` generado. Si realiza la generación del formato `.png` nuevamente, estos se sobreescribirán.

## Estructura del proyecto
El proyecto se encuentra distribuido de la siguiente manera:

|---ContextMap

|---|--- pda-context-mapper-as-is.cml

|---|--- pda-context-mapper-as-is.cml

|--- src-gen

|---|--- pda-context-mapper-as-is_ContextMap.png

|---|--- pda-context-mapper-to-be_ContextMap.png

|--- README.md

## Distribución archivo .cml
1. **Documentación de dominios y subdominios:** La documentación de los dominios y subdominios se encuentra en el archivo `pda-context-mapper` para cada uno de los modelos AS-IS y TO-BE. En la primera parte del código se puede ver la definición del dominio y los subdominios, con sus respectivos tipos y _Vision Statement_.
2. **Documentacion de lenguaje ubicuo:** La siguiente imagen muestra el resultado del EventStorming para el flujo "adquisición y enriquecimiento de datos automatizado".
   
* [Modelo AS-IS](https://raw.githubusercontent.com/monicabajonerodcastro/Inseparables-AppsNoMonoliticas/main/assets/ASIS.png)
  
* [Modelo TO-BE](https://raw.githubusercontent.com/monicabajonerodcastro/Inseparables-AppsNoMonoliticas/main/assets/TOBE.png)
  
Si desea ver la documentación en su formato original y/o en una mayor resolución, podra encontrarla en [este link](https://miro.com/app/board/uXjVNxpr2Xs=/?share_link_id=625882265572).

3. Documentación de contextos acotados: La documentación de los contextos acotados se encuentra en el archivo `pda-context-mapper` para cada uno de los modelos AS-IS y TO-BE. En la segunda sección del código, se puede ver la definición de los contextos con sus respectivas relaciones y _Vision Statement_.
