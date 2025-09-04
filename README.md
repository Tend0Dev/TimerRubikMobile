# TimerRubik 🎲⏱️

Una aplicación de temporizador para cubo de Rubik desarrollada en Flutter, diseñada para speedcubers que quieren mejorar sus tiempos y aprender algoritmos.

## 📱 Características

- **⏱️ Temporizador de alta precisión**: Cronómetro preciso con decimales para medir tus soluciones
- **🔀 Generador de scrambles**: Genera mezclas aleatorias para cada intento
- **📊 Registro de tiempos**: Guarda y visualiza historial completo de tus tiempos
- **📚 Algoritmos OLL y PLL**: Aprende los algoritmos esenciales con diagramas visuales
- **📱 Multiplataforma**: Disponible para Android, iOS, Web, Windows, macOS y Linux
- **🎨 Interfaz moderna**: Diseño intuitivo y fácil de usar

## 🚀 Instalación

### Prerrequisitos

- [Flutter SDK](https://flutter.dev/docs/get-started/install) (versión 3.3.0 o superior)
- Dart SDK incluido con Flutter
- Un editor de código (recomendado: VS Code, Android Studio)

### Pasos de instalación

1. **Clona el repositorio**
   ```bash
   git clone https://github.com/Tend0Dev/TimerRubik.git
   cd TimerRubik
   ```

2. **Instala las dependencias**
   ```bash
   flutter pub get
   ```

3. **Ejecuta la aplicación**
   ```bash
   flutter run
   ```

## 🏗️ Estructura del Proyecto

```
lib/
├── main.dart                    # Punto de entrada de la aplicación
├── providers/                   # Gestión de estado con Provider
│   ├── times_providers.dart     # Proveedor para gestión de tiempos
│   └── scramble_providers.dart  # Proveedor para gestión de scrambles
├── screens/                     # Pantallas principales
│   ├── onboarding_screen.dart   # Pantalla principal con navegación
│   ├── algorithms_screen.dart   # Pantalla de algoritmos
│   ├── list_views.dart          # Vista de listas
│   └── rubik_timer.dart         # Pantalla del temporizador
├── views/                       # Componentes de vista
│   ├── rubik_timer.dart         # Vista del temporizador
│   ├── records.dart             # Vista de registros
│   ├── algorithms_oll.dart      # Algoritmos OLL
│   ├── algorithms_pll.dart      # Algoritmos PLL
│   ├── scramble.dart            # Generador de scrambles
│   └── side_menu.dart           # Menú lateral
└── widgets/                     # Widgets reutilizables
    └── custom_app_bar.dart      # Barra de aplicación personalizada

assets/                          # Recursos estáticos
├── *.png                        # Diagramas de algoritmos
└── banner.jpeg                  # Banner de la aplicación
```

## 🎮 Cómo usar

### Temporizador
1. Observa el scramble generado automáticamente
2. Prepara tu cubo según la mezcla mostrada
3. Toca la pantalla para iniciar el cronómetro
4. Resuelve el cubo lo más rápido posible
5. Toca nuevamente para detener el tiempo
6. Tu tiempo se guardará automáticamente

### Algoritmos
- Navega por los algoritmos OLL (Orientation of the Last Layer)
- Explora los algoritmos PLL (Permutation of the Last Layer)
- Cada algoritmo incluye diagramas visuales para facilitar el aprendizaje

### Historial de Tiempos
- Revisa todos tus tiempos anteriores
- Analiza tu progreso y mejoras

## 🛠️ Desarrollo

### Dependencias principales

- **flutter**: Framework de desarrollo
- **provider**: Gestión de estado
- **shared_preferences**: Almacenamiento local
- **cupertino_icons**: Iconos de iOS

### Comandos útiles

```bash
# Ejecutar en modo debug
flutter run

# Construir para release
flutter build apk          # Android
flutter build ios          # iOS
flutter build web          # Web

# Ejecutar tests
flutter test

# Analizar código
flutter analyze
```

### Contribuir

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/nueva-caracteristica`)
3. Commit tus cambios (`git commit -am 'Agrega nueva característica'`)
4. Push a la rama (`git push origin feature/nueva-caracteristica`)
5. Abre un Pull Request

## 📋 Roadmap

- [ ] Estadísticas avanzadas (promedio de 5, promedio de 12)
- [ ] Gráficos de progreso
- [ ] Diferentes tipos de scrambles (2x2, 4x4, etc.)
- [ ] Modo competición
- [ ] Sincronización en la nube
- [ ] Más algoritmos (ZBLL, COLL, etc.)

## 🐛 Reportar Bugs

Si encuentras algún error, por favor crea un [issue](https://github.com/Tend0Dev/TimerRubik/issues) con:
- Descripción del problema
- Pasos para reproducirlo
- Capturas de pantalla (si aplica)
- Información del dispositivo

## 📄 Licencia

Este proyecto está bajo la licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 👨‍💻 Autor

**Tend0Dev** - [GitHub](https://github.com/Tend0Dev)

---

¡Si te gusta el proyecto, no olvides darle una ⭐ en GitHub!
