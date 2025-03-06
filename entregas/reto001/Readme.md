# Análisis de Código Java

## Código Elcaracol  
[Enlace al código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Elcaracol.java)  

### 1. Nombres Incorrectos o Poco Descriptivos  
- **Línea 2**: `Elcaracol` → Nombre críptico (no revela propósito).  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Elcaracol.java#L2)  
- **Líneas 5-6**: `n`, `m` → Nombres genéricos (no indican qué representan).  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Elcaracol.java#L5-L6)  
- **Líneas 7-8**: `i`, `j` → Nombres de variables de bucle poco descriptivos.  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Elcaracol.java#L7-L8)  

### 2. Variables No Utilizadas  
No se detectan variables no utilizadas en este código.  

### 3. Lógica Estructural Incorrecta  
- **Líneas 10-15**: Bucles `for` anidados para llenar la matriz → No hay validación de límites de la matriz.  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Elcaracol.java#L10-L15)  
- **Líneas 17-22**: Bucles `for` para imprimir la matriz → Código repetitivo que podría extraerse en un método.  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Elcaracol.java#L17-L22)  

### 4. Nombres de Variables Confusos  
- **Líneas 5-6**: `n`, `m` → No queda claro si representan filas, columnas o algún otro valor.  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Elcaracol.java#L5-L6)  

### 5. Convenciones de Java Incumplidas  
- **Línea 3**: Clase `main` con toda la lógica → Debería dividirse en métodos.  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Elcaracol.java#L3)  
- **Líneas 10-22**: Código repetitivo para llenar e imprimir la matriz → Falta de modularidad.  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Elcaracol.java#L10-L22)  

### 6. Errores de Semántica  
- **Líneas 10-15**: No hay validación de que `n` y `m` sean valores positivos.  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Elcaracol.java#L10-L15)  

---

## Código RetoCCCF  
[Enlace al código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/RetoCCCF.java)  

### 1. Nombres Incorrectos o Poco Descriptivos  
- **Línea 2**: `RetoCCCF` → Nombre críptico (no revela propósito).  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/RetoCCCF.java#L2)  
- **Líneas 5-9**: `caja1`, `caja2`, etc. → Nombres genéricos (no indican qué almacenan).  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/RetoCCCF.java#L5-L9)  
- **Línea 10**: `colaCero` → Confuso (cuenta minutos sin clientes).  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/RetoCCCF.java#L10)  

### 2. Variables No Utilizadas  
- **Línea 15**: `compra` → Declarada pero nunca usada.  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/RetoCCCF.java#L15)  

### 3. Lógica Estructural Incorrecta  
- **Línea 16**: Bucle `for` procesa minutos, pero las cajas (líneas 21-58) están fuera del bucle → Se ejecutan una sola vez (error crítico).  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/RetoCCCF.java#L16)  

---

## Código Whacamole  
[Enlace al código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Whacamole.java)  

### 1. Nombres Poco Descriptivos  
- **Línea 3**: `Whacamole` → No sigue `CamelCase` (debería ser `WhacAMole`).  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Whacamole.java#L3)  
- **Línea 9**: `monigote`, `monigote1` → Nombres en español y no revelan su propósito (deberían ser `molePosition1`, `molePosition2`).  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Whacamole.java#L9)  

### 2. Variables con Nombres Confusos  
- **Línea 10**: `contador` → Usado para numerar celdas, pero su nombre no lo refleja (mejor `currentCell`).  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Whacamole.java#L10)  

### 3. Números sin Constantes  
- **Línea 5**: `4` → Tamaño del tablero "hardcodeado" (debería ser `final int GRID_SIZE = 4;`).  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Whacamole.java#L5)  

### 4. Lógica Redundante  
- **Líneas 29 y 35**: Código duplicado para verificar `monigote` y `monigote1` (debería usarse un array o método).  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Whacamole.java#L29)  

### 5. Validación de Entrada Incorrecta  
- **Líneas 19-22**: El `do-while` permite `casilla = 0` (inválido). La condición debe ser `casilla < 1 || casilla > 16`.  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Whacamole.java#L19-L22)  

### 6. Inconsistencia en Idioma  
- Variables en español (`turno`, `acierto`, `casilla`) en un contexto de código que debería ser en inglés.  
  [Ver código](https://github.com/pabloocanteroo/prg1-22-23/blob/main/retos/entregas/Whacamole.java#L6-L8)  
