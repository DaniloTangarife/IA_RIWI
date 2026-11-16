# Prototipo MVP - Gestión de Inventario y Preventa Textil ("Divina Providencia")

Acceso directo al prototipo funcional desplegado en Vercel:
👉 **[Abrir Aplicación en Vivo](https://divina-providencia-prototipo-mvp-6f.vercel.app/)**

---

## 🎯 ¿Qué hace esta página?
Este prototipo materializa la solución digital para pequeñas empresas y bodegas del sector textil (tomando como piloto a **Divina Providencia** en Medellín)[cite: 3]. Su objetivo es digitalizar el ciclo ineficiente de preventa en ruta y control de inventarios, eliminando el uso de Excel manual y talonarios de papel para evitar sobreventas y errores humanos[cite: 3].

## 📱 Componentes Clave para Evaluar (TL View)

El prototipo integra los flujos principales definidos en la especificación técnica del negocio:

1. **Panel Web de Administración (Bodega):**
   * **Kardex de Inventario:** Visualización de stock con estados claros (*Disponible, Stock Bajo, Agotado*)[cite: 4].
   * **Carga Masiva:** Interfaz optimizada para la importación y validación de archivos de inventario (`.csv` / `.xlsx`) estructurados por matriz de tallas y colores[cite: 4].
   * **Supervisión de Pedidos:** Gestión por pestañas (*Pendientes / Despachados*) para control logístico en bodega[cite: 4].

2. **App Móvil / Interfaz de Preventa (Vendedor en Ruta):**
   * **Matriz Interactiva de Variantes:** Selector dinámico por color y cuadrícula de tallas con indicador de stock en tiempo real[cite: 4].
   * **Cierre de Pedido:** Resumen consolidado de transacciones con opciones de envío rápido[cite: 4].

## 🛠️ Stack Tecnológico de Referencia
* **Frontend Web:** React.js con Tailwind CSS[cite: 3].
* **Frontend Móvil:** React Native (Expo)[cite: 3].
* **Backend & API:** Python con FastAPI (Procesamiento concurrente y documentación en Swagger)[cite: 3].
* **Base de Datos:** PostgreSQL (Garantía de integridad transaccional con `with_for_update()` para evitar sobreventas)[cite: 3, 4].