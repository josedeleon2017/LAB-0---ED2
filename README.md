# LABORATORIO #0

### José Vinicio De León Jiménez

1072619

Objetivos:
- Aprender el concepto de tareas y proyectos por cumplir
- Comprender la estructura de un JSON
- Utilizar una API a través de un cliente Web

### SERIE II

En la implementación de la serie II se seleccionó el escenario de las clases como una empresa de electrodomésticos, en donde la empresa contenía distintas sucursales representadas por la clase tienda. La clase tienda contiene a la vez la clase persona además de sus propiedades específicas, luego la clase persona contiene la clase ventas. Esta implementación es un ejemplo sencillo de la abstracción y asociación de datos.

![LABORATORIO%20#0%200825b0ef72564c58b0db86f8cc8d8f0e/diagrama.png](LABORATORIO%20#0%200825b0ef72564c58b0db86f8cc8d8f0e/diagrama.png)

### SERIE III

En esta sección se hicieron peticiones en APIDemo, una API basada en el tipo de cambio entre quetzales y dólares. Las peticiones fueron las siguientes.

- Consulta de toda la lista de tipos de cambio: GET api/exchangerate
- Consulta de toda la lista de tipo de cambio cambiando la moneda base: GET api/exchangerate?BaseCurrency=usd
- Consulta de tipo de cambio de una fecha específica: GET api/exchangerate/{date}
- Insertar tipo de cambio para un nuevo dia: POST api/exchangerate
- Actualizar información de tipo de cambio para un día: PUT api/exchangerate/{date}
- Eliminar información de tipo de cambio de un día: DELETE api/exchangerate/{date}

**Insert**

![LABORATORIO%20#0%200825b0ef72564c58b0db86f8cc8d8f0e/post.png](LABORATORIO%20#0%200825b0ef72564c58b0db86f8cc8d8f0e/post.png)

Como se puede observar en la imagen, a través del método POST se realiza la inserción del objeto JSON especificado.

**Update**

![LABORATORIO%20#0%200825b0ef72564c58b0db86f8cc8d8f0e/put_1.png](LABORATORIO%20#0%200825b0ef72564c58b0db86f8cc8d8f0e/put_1.png)

Al hacer uso del método PUT, modificando el objeto JSON en el body y especificando la fecha del objeto a actualizar en la URL se envía la petición sin aparentemente ningún resultado.

![LABORATORIO%20#0%200825b0ef72564c58b0db86f8cc8d8f0e/put_2.png](LABORATORIO%20#0%200825b0ef72564c58b0db86f8cc8d8f0e/put_2.png)

Al hacer la consulta de los objetos cargados en la API podemos verificar que efectivamente el valor cambió.

**DELETE**

![LABORATORIO%20#0%200825b0ef72564c58b0db86f8cc8d8f0e/delete_real.png](LABORATORIO%20#0%200825b0ef72564c58b0db86f8cc8d8f0e/delete_real.png)

Al hacer uso del método DELETE, se eliminó el objeto de la fecha especificada en la URL de POSTMAN.

![LABORATORIO%20#0%200825b0ef72564c58b0db86f8cc8d8f0e/put_2.png](LABORATORIO%20#0%200825b0ef72564c58b0db86f8cc8d8f0e/put_2.png)

Al hacer la consulta de los objetos cargados en la API podemos verificar que efectivamente el valor fue eliminado.
