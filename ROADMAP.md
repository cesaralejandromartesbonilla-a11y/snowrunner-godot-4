# 🗺️ Hoja de Ruta (Roadmap) — SnowRunner Godot 4

Este documento define la trayectoria técnica de expansión de mecánicas todoterreno, deformación de terreno y simulación de tren motriz en Godot 4.

---

## 📌 Fase 1: Núcleo de Simulación y Logística (Completado ✅)
- [x] Singleton de gestión de garaje (`GestionGaraje.gd`) y cambio de vehículos.
- [x] Áreas de fango (`MudArea.gd`) con reducción de tracción e incremento de arrastre.
- [x] Zonas de carga de mercancías y entrega en puntos de construcción.
- [x] Camión grúa y camioneta heavy integrados.
- [x] Limpieza de caché no versionable `.godot`.

---

## 📌 Fase 2: Deformación Real de Huellas y Terreno Volumétrico (En Progreso 🔄)
- [ ] **Desplazamiento Dinámico de Huellas por Shader de Terreno**:
  - Grabado de huellas de neumáticos (*tire tracks displacement*) en mapas de altura de textura en tiempo real.
- [ ] **Tren Motriz Detallado (Powertrain Simulation)**:
  - Marchas cortas (*Low Gear* $L, L+, L-$) para torque máximo sin patinar.
  - Bloqueo manual de diferencial (Diff Lock) con penalización de radio de giro.
  - Consumo de combustible dinámico basado en RPM y carga del motor.
- [ ] **Sistema de Cabrestante de Rescate (Winch Physics)**:
  - Anclaje a árboles y postes cercanos con cálculo de resistencia a la tracción.

---

## 📌 Fase 3: Meteorología y Misiones de Campaña 🚀
- [ ] **Ciclo Día/Noche y Clima Dinámico**:
  - Lluvia torrencial que convierte caminos de tierra seca en lodo profundo.
  - Niebla densa y nieve acumulativa.
- [ ] **Generador Procedural de Contratos**:
  - Misiones aleatorias de recuperación de vehículos volcados y abastecimiento de combustible a campamentos remotos.
