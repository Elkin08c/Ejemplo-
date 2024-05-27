# Tarea en Clase Semana-8
## La funcion Count
### creacion de la Tabla
El siguinet ecodigo Genrea la tabla **client**
```
CREATE TABLE client(
id SERIAL
nui VARCHAR(11) NO NULL,
fullname VARCHAR(100) NOT NULL,
phone VARCHAR(10),
type_of_client VARCHAR (50) DEFAULT 'BASIC',
city VARCHAR(50),
credit_limit DECIMAL (7,2)
);
```
### Insercion de Datos
```
INSERT INTO client (nui, fullname, phone, type_of_client, city, credit_limit) VALUES
('01020304050', 'Juan Perez', '0991234567', 'PREMIUM', 'Guayaquil', 1500.00),
('02030405060', 'Maria Gomez', '0987654321', 'BASIC', 'Cuenca', 1200.00),
('03040506070', 'Carlos Sanchez', '0971234567', 'GOLD', 'Manta', 2000.00),
('04050607080', 'Ana Morales', '0967654321', 'SILVER', 'Quito', 1000.00),
('05060708090', 'Luis Fernandez', '0951234567', 'BASIC', 'Guayaquil', 1300.00),
('06070809010', 'Martha Lopez', '0947654321', 'PREMIUM', 'Cuenca', 2500.00),
('07080901020', 'Pedro Ramirez', '0931234567', 'GOLD', 'Manta', 2200.00),
('08091011230', 'Laura Diaz', '0927654321', 'SILVER', 'Quito', 1100.00),
('09101112140', 'Jorge Ortiz', '0911234567', 'BASIC', 'Guayaquil', 1400.00),
('10111213150', 'Sofia Chavez', '0907654321', 'PREMIUM', 'Cuenca', 1600.00);

```

### Mostrar el total de Nombres
Para mostrar todos los nombres usamos la funcion **COUNT ()** pasandole commo un paramatre el campo , en este caso  *fullname*
```
SELECT COUNT (fullname) AS total_names 
FROM client;
```
- Capturas

<img src="../capturas/COUNT-1.png" width="500"/>
