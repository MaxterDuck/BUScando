# Empresa: BUScando

## ✨ Nombre del producto
**BUScando** - La app que conecta usuarios, conductores y supervisores del transporte público en tiempo real.

---

## 🔀 Roles y entregables

### 👥 Product Owner - Requisitos
Problema que resuelve: La incertidumbre sobre la llegada del transporte público, pérdida de tiempo en paraderos y falta de comunicación entre usuarios, conductores y supervisores.

Público objetivo: -Usuarios del transporte público
-Conductores de buses
-Supervisores del sistema de transporte

3 funcionalidades clave:
i. Visualización en tiempo real del bus y su ubicación actual
 ii. Canal de reporte de novedades por parte del conductor (tráfico, incidentes, retrasos)
 iii. Panel de control para el supervisor con acceso a estadísticas, recorridos y estado en vivo, chat en tiempo real con el conductor.


### 📊 Analista - Análisis
- **Tareas**:
  - Configurar sesiones de temporizador.
  - Vincular metas y recompensas.
  - Crear sistema de historial con gráficas.
- **Dificultad estimada**:
  - Temporizador: media
  - Recompensas: alta
  - Historial: media
- **Restricciones**:
  - Solo funciona sin conexión a internet.
  - Interfaz ultra simple, sin distracciones.

### 🎨 Diseñador UX/UI - Bocetos y flujo
- **Pantalla 1**: Temporizador activo con selector de sonido (mar, bosque, silencio).
- **Pantalla 2**: Panel de progreso con metas y recompensas desbloqueadas.
- **Flujo**:
  Inicio → Elegir sesión → Iniciar foco → Recompensa → Historial

### 🛠️ Desarrollador - Implementación
- **Feature implementada**: Temporizador con selector de sonido
- **Pseudocódigo**:
```ruby
if session.start?
  play_sound(selected)
  start_timer(25.minutes)
end
```
- **Tecnología**: Flutter para app multiplataforma

### 🔧 QA Tester - Pruebas
- **Caso 1**: Al iniciar sesión, el temporizador inicia correctamente
- **Caso 2**: Al finalizar, se activa sonido de "tarea cumplida"
- **Caso 3**: Si se cancela la sesión, el temporizador se reinicia
- **Errores esperados**:
  - No carga sonidos si hay permisos denegados
  - El historial no guarda si la sesión fue muy corta (<5 min)

### 📦 DevOps/Mantenimiento - Despliegue
- **Despliegue**:
  - En Google Play y App Store usando Codemagic CI/CD
  - Almacenamiento local de sesiones (sin backend)
- **2 mejoras futuras**:
  1. Sincronización con nube para respaldos
  2. Integración con calendarios personales

---

## 📅 Herramientas utilizadas
- **Diseño**: Figma
- **Documentación**: Google Docs + README.md
- **Presentación**: Canva + exposición oral

---

## 🌟 Ejemplo de presentación (pitch 2 min)
> "Hola, somos el equipo de FocusZen. Creamos una app simple para ayudar a estudiantes como nosotros a mantener la concentración. Tiene sonidos de ambiente, temporizador Pomodoro y un sistema visual de logros. Nuestra propuesta se basa en mejorar hábitos sin generar dependencia digital. Diseñamos dos pantallas principales, con una experiencia limpia y motivadora. En el futuro queremos integrarla con Google Calendar y crear rankings entre amigos."

---
