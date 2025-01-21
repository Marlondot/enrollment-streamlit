# enrollment-streamlit

Como prueba de concepto se espera usar [streamlit](https://streamlit.io/) como una especie de front para llevar funcionalidades de contabilidad y registro de usuarios

## ¿Qué tipo de funcionalidades?

Como primera idea, podemos imaginar la funcionalidad de un contador, en la que el usuario introduce un número entero y al pulsar un botón de guardar dicho dato se envía a una base de datos que guarda la fecha en la que ocurrió el guardado, y el número asociado. 

A pesar de que en un principio suene básico, esto podría funcionar como base para un sistema que guarde asistencias dados números de identificación.

## ¿Cómo hacerlo?

### Streamlit

Para comenzar se puede revisar la documentación de streamlit, específicamente para los [input widgets](https://docs.streamlit.io/develop/api-reference/widgets/st.number_input), a partir de los cuales se puede incluir la funcionalidad principal.

### Testing

Se puede pensar en incluir testing. Por una parte, los tests van a ser más fáciles de hacer mientras más [desacoplada](https://softwareengineering.stackexchange.com/a/244478) se encuentre toda la aplicación, es decir: no poner todo sobre una misma función, tratar de dividir por funcionalidades.

Por otra parte Streamlit tiene su [propio módulo](https://docs.streamlit.io/develop/api-reference/app-testing/testing-element-classes#sttestingv1element_treenumberinput) de testeo para emular las funcionalidades de los widgets presentes. Se puede juntar con [pytest](https://docs.pytest.org/en/stable/getting-started.html#create-your-first-test) para hacer tests unitarios (probar funcionalidades básicas).


### Base de datos

Para pruebas locales se puede crear una [conexión local MySQL](https://github.com/Lunes313/StreamlitProyect/blob/main/database.py)

Además para probar con una base de datos en nube se puede usar la [capa gratuita de MongoDB](https://www.mongodb.com/pricing) 

También se pueden buscar otras maneras de hosting para bases de datos en [foros](https://www.reddit.com/r/webdev/comments/vc2hpc/any_websites_where_i_can_host_sqlite_db_for_free/), la  idea es no cerrarse a explorar

## Tareas

- [x] Primera tarea
