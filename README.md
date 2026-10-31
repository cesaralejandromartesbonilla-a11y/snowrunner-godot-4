# 🚛 SnowRunner Godot 4 — Off-Road Heavy Logistics Simulator

Simulador de logística pesada, transporte todoterreno y física de vehículos en terreno difícil para **Godot 4.5 / 4.x**, inspirado en las mecánicas de *SnowRunner* y *MudRunner*.

---

## 🌟 Características Principales

- **Física de Terreno Deformable y Barro (`MudArea.gd`)**:
  - Detección de hundimiento de neumáticos según par de giro, peso del vehículo y tipo de tracción (AWD / bloqueo de diferencial).
  - Resistencia al avance y pérdida de tracción en áreas de fango y nieve.
- **Flota de Vehículos Pesados (`vehicles/`)**:
  - Camioneta pickup de carga pesada (`camioneta_heavy.tscn`).
  - Camión grúa de rescate (`grua.tscn`) con brazo articulado y puntos de enganche.
  - Sistema de remolques y enganches de quinta rueda (`remolques/`).
- **Sistema de Gestión de Garajes y Flota (`GestionGaraje.gd` y `UI_Garaje.gd`)**:
  - Almacén de vehículos, cambio de camión activo, reparación y repostaje en gasolinera (`Gasolinera.gd`).
- **Contratos de Construcción y Puntos de Carga**:
  - Zonas de carga de materiales (`ZonaCarga.gd`).
  - Sitios de construcción dinámicos (`sitio_construccion.gd`, `SitioConstruccionSpawner.gd`) con progreso de entrega y culminación de estructuras (`edificaciones/edificio_terminado.tscn`).

---

## 📂 Estructura del Proyecto

```text
snowrunner-godot-4/
├── edificaciones/               # Estructuras entregables y garajes
│   ├── Garage.tscn
│   └── edificio_terminado.tscn
├── remolques/                   # Remolques de carga de troncos y carga general
├── vehicles/                    # Modelos y física de camiones y camionetas
│   ├── camioneta_heavy.tscn
│   └── grua.tscn
├── Garage.gd                    # Lógica de interacción en el taller
├── GestionGaraje.gd             # Singleton autoload de inventario y estado
├── MudArea.gd                   # Áreas físicas de lodo con fricción reducida
├── Gasolinera.gd                # Reabastecimiento de combustible
├── ZonaCarga.gd                 # Spawner y receptor de carga/pallets
├── main.tscn                    # Mapa principal todoterreno
├── project.godot                # Configuración de Godot 4.5 Forward Plus
├── README.md                    # Documentación
└── ROADMAP.md                   # Hoja de ruta técnica
```

---

## 🚀 Requisitos y Uso

1. **Versión de Godot**: Godot Engine 4.3+ / 4.5+ (Renderer Forward Plus).
2. **Ejecución**:
   - Abre Godot y carga la carpeta del proyecto.
   - Ejecuta la escena principal (`main.tscn`) con `F5`.
   - Conduce con `W, A, S, D` o flechas de dirección. Interactúa con las zonas de carga para aceptar contratos de entrega.

---

## 📄 Licencia

Código abierto bajo licencia MIT.
