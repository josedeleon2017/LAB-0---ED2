# LABORATORIO #0

### José Vinicio De León Jiménez

1072619

Objetivos:
- Aprender el concepto de tareas y proyectos por cumplir
- Comprender la estructura de un JSON
- Utilizar una API a través de un cliente Web

### SERIE II

En la implementación de la serie II se seleccionó el escenario de las clases como una empresa de electrodomésticos, en donde la empresa contenía distintas sucursales representadas por la clase tienda. La clase tienda contiene a la vez la clase persona además de sus propiedades específicas, luego la clase persona contiene la clase ventas. Esta implementación es un ejemplo sencillo de la abstracción y asociación de datos.

<img src="https://github.com/josedeleon2017/LAB-0---ED2/blob/master/SERIE%20II/diagrama.png" width="500" height="150"/>

 
### SERIE III

En esta sección se hicieron peticiones en APIDemo, una API basada en el tipo de cambio entre quetzales y dólares. Las peticiones fueron las siguientes.

- Consulta de toda la lista de tipos de cambio: GET api/exchangerate
- Consulta de toda la lista de tipo de cambio cambiando la moneda base: GET api/exchangerate?BaseCurrency=usd
- Consulta de tipo de cambio de una fecha específica: GET api/exchangerate/{date}
- Insertar tipo de cambio para un nuevo dia: POST api/exchangerate
- Actualizar información de tipo de cambio para un día: PUT api/exchangerate/{date}
- Eliminar información de tipo de cambio de un día: DELETE api/exchangerate/{date}

**REQUESTS**
```
https://localhost:44332/api/exchangerate
```
<img src="https://github.com/josedeleon2017/LAB-0---ED2/blob/master/SERIE%20III/requests%20images/request%201.PNG"/>

```
https://localhost:44332/api/exchangerate?BaseCurrency=gtq
https://localhost:44332/api/exchangerate?BaseCurrency=usd
```

<img src="https://github.com/josedeleon2017/LAB-0---ED2/blob/master/SERIE%20III/requests%20images/get%202.PNG"/>

```
https://localhost:44332/api/exchangerate/2020-08-05
```

<img src="https://github.com/josedeleon2017/LAB-0---ED2/blob/master/SERIE%20III/requests%20images/get%203.PNG"/>

**INSERT**
```
https://localhost:44332/api/exchangerate

{
  "id": 7,
  "date": "2020-08-26T00:00:00",
  "usd": 9.5,
  "gtq": 1
}
```

<img src="https://github.com/josedeleon2017/LAB-0---ED2/blob/master/SERIE%20III/requests%20images/post.png"/>

Como se puede observar en la imagen, a través del método POST se realiza la inserción del objeto JSON especificado.

**UPDATE**
```
https://localhost:44332/api/exchangerate/2020-08-25
```

<img src="https://github.com/josedeleon2017/LAB-0---ED2/blob/master/SERIE%20III/requests%20images/put%201.PNG"/>

Al hacer uso del método PUT, modificando el objeto JSON en el body y especificando la fecha del objeto a actualizar en la URL se envía la petición sin aparentemente ningún resultado.

<img src="https://github.com/josedeleon2017/LAB-0---ED2/blob/master/SERIE%20III/requests%20images/put%202.PNG"/>

Al hacer la consulta de los objetos cargados en la API podemos verificar que efectivamente el valor cambió.

**DELETE**
```
https://localhost:44332/api/exchangerate/2020-08-25
```

<img src="https://github.com/josedeleon2017/LAB-0---ED2/blob/master/SERIE%20III/requests%20images/delete%201.PNG"/>

Al hacer uso del método DELETE, se eliminó el objeto de la fecha especificada en la URL de POSTMAN.

<img src="https://github.com/josedeleon2017/LAB-0---ED2/blob/master/SERIE%20III/requests%20images/delete%202.PNG"/>

Al hacer la consulta de los objetos cargados en la API podemos verificar que efectivamente el valor fue eliminado.
