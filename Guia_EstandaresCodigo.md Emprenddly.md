#  Guia_EstandaresCodigo.md

##  Stack del proyecto

- **Frontend móvil:** React Native   
- **Backend:** Python (FastAPI + SQLAlchemy)  
- **Base de datos:** PostgreSQL  
- **Herramientas de desarrollo:**  VSCode, Git, Expo

---

## a.  Reglas de nombres

### Python (FastAPI)

- Variables: `snake_case`
- Funciones y métodos: `snake_case`
- Clases: `PascalCase`
- Constantes: `UPPER_SNAKE_CASE`
- Archivos: `snake_case.py`

**Ejemplo:**
```python
class ProductoInventario:
    def calcular_total(self, cantidad, precio_unitario):
        total = cantidad * precio_unitario
        return total

 const InventarioCard = ({ nombreProducto }) => {
  return <Text>{nombreProducto}</Text>;
}

def obtener_producto(id: int) -> Producto:
    """
    Retorna un producto dado su ID.
    """
    return db.query(Producto).filter(Producto.id == id).first()
// Componente que muestra la información del inventario
const InventarioCard = () => {
  /** Muestra el nombre del producto y su cantidad disponible */
  return <Text>Producto</Text>;
}
class ReporteVentas(BaseModel):
    fecha: date
    total: float
class reporte:
    Fecha = ""
    Total = 0
const BotonGuardar = () => {
  return <Button title="Guardar" onPress={handleGuardar} />;
}
function boton() {
  return <button>guardar</button>;
}
sudo apt install nodejs npm
npx create-expo-app nombre-app
python -m venv env
source env/bin/activate  # Linux/macOS
env\\Scripts\\activate   # Windows
pip install fastapi sqlalchemy psycopg2 uvicorn
uvicorn main:app  reload
SQLALCHEMY_DATABASE_URL = "postgresql://usuario:clave@localhost/db"
engine = create_engine(SQLALCHEMY_DATABASE_URL)







