#  Guía  de Código

Este documento define los criterios de escritura del código, nomenclatura, estilo  para el desarrollo de la  aplicación móvil de contabilidad e inventario para microempresas.

---

## 1. Reglas de Nomenclatura

###  Frontend – React Native (JavaScript/TypeScript)

- **Variables y funciones:** camelCase  
  Ej: `totalVenta`, `calcularSubtotal()`

- **Componentes:** PascalCase  
  Ej: `FormularioProducto`, `ResumenVentas`

- **Archivos:** kebab-case o camelCase  
  Ej: `registro-usuario.js`, `detalleProducto.tsx`

###  Backend – FastAPI (Python)

- **Variables y funciones:** snake_case  
  Ej: `obtener_datos()`, `cliente_id`

- **Clases:** PascalCase  
  Ej: `UsuarioModel`, `InventarioService`

- **Archivos:** snake_case  
  Ej: `ventas_api.py`, `conexion_bd.py`

---

## 2. Comentarios y Documentación

###  React Native

- Usar `//` para comentarios breves y `/** ... */` para documentar componentes o funciones.

```js
// Calcula el total de la venta
function calcularTotal(precio, cantidad) {
  return precio * cantidad;
}
```

###  FastAPI

- Usar docstrings con triple comilla `"""` para documentar funciones y clases.

```python
def registrar_usuario():
    """
    Registra un nuevo usuario en la base de datos.
    """
    pass
```

- Comentar lógica compleja cuando sea necesario.

---

## 3.  Estilo e Identación

### General

- **Espacios:**
  - 2 espacios para JavaScript/TypeScript
  - 4 espacios para Python

- **Comillas:**
  - Simples (') en JS/TS
  - Dobles (") en Python

- **Longitud máxima por línea:** 120 caracteres

- **Llaves:** Siempre en la misma línea que la declaración

---

## 4. Ejemplos Aceptados /  No Aceptados

### 📱 React Native

**  Aceptado:**
```js
const nombreUsuario = 'Carlos';

function obtenerTotal(precio, cantidad) {
  return precio * cantidad;
}
```

** No Aceptado:**
```js
var x = 'Carlos';
function OBTENERTOTAL(P,C){ return P*C; }
```

---

### FastAPI (Python)

**Aceptado:**
```python
def calcular_total(precio, cantidad):
    return precio * cantidad
```

**No Aceptado:**
```python
def Total(P,C): return P*C
```

---

## 5. Herramientas de Formato y Estilo

###  React Native

Instalar linters y formateadores:
```bash
npm install eslint prettier eslint-config-prettier eslint-plugin-react eslint-plugin-react-native --save-dev
```

Comandos para corregir automáticamente:
```bash
npx eslint . --fix
npx prettier --write .
```

###  FastAPI (Python)

Instalar herramientas:
```bash
pip install black flake8 isort
```

Comandos:
```bash
black .
flake8 .
isort .
```

---

## 6.  Reglas de Aplicacion

- Todas las reglas aquí escritas deben aplicarse al código nuevo.
- El código que ya debe ser modificado para cumplir con estas reglas  usando los linters y formateadores que  favorables para el proyecto.
- Esta guía debe mantenerse actualizada a medida que avance el proyecto.



