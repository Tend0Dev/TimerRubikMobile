# Guía de Configuración para Desarrollo

Esta guía te ayudará a configurar el entorno de desarrollo para TimerRubik.

## 📋 Prerrequisitos

### 1. Flutter SDK
Instala Flutter SDK desde [flutter.dev](https://flutter.dev/docs/get-started/install)

**Windows:**
```bash
# Descargar Flutter SDK
# Agregar Flutter al PATH del sistema
flutter doctor
```

**macOS:**
```bash
# Usar Homebrew (recomendado)
brew install flutter

# O descargar manualmente desde flutter.dev
flutter doctor
```

**Linux:**
```bash
# Descargar Flutter SDK
wget https://storage.googleapis.com/flutter_infra_release/releases/stable/linux/flutter_linux_3.x.x-stable.tar.xz
tar xf flutter_linux_3.x.x-stable.tar.xz
export PATH="$PATH:`pwd`/flutter/bin"
flutter doctor
```

### 2. Editores recomendados

**Visual Studio Code**
```bash
# Instalar VS Code
# Extensiones recomendadas:
# - Flutter
# - Dart
# - Flutter Widget Snippets
# - Awesome Flutter Snippets
```

**Android Studio**
```bash
# Instalar Android Studio
# Plugins recomendados:
# - Flutter
# - Dart
```

### 3. Configuración de plataformas

**Android**
- Android Studio o Android SDK
- Java Development Kit (JDK) 8 o superior
- Android SDK Platform Tools

**iOS (solo macOS)**
- Xcode 12 o superior
- CocoaPods: `sudo gem install cocoapods`

**Web**
- Chrome (para depuración)

## 🚀 Configuración del Proyecto

### 1. Clonar y configurar
```bash
# Clonar el repositorio
git clone https://github.com/Tend0Dev/TimerRubik.git
cd TimerRubik

# Verificar configuración de Flutter
flutter doctor

# Instalar dependencias
flutter pub get

# Verificar que todo funciona
flutter analyze
```

### 2. Configuración específica por plataforma

**Android:**
```bash
# Crear archivo local.properties en android/
echo "sdk.dir=/path/to/Android/Sdk" > android/local.properties

# Ejecutar en emulador/dispositivo Android
flutter run
```

**iOS (macOS únicamente):**
```bash
# Instalar dependencias de iOS
cd ios
pod install
cd ..

# Ejecutar en simulador iOS
flutter run
```

**Web:**
```bash
# Habilitar soporte web (si no está habilitado)
flutter config --enable-web

# Ejecutar en web
flutter run -d chrome
```

## 🛠️ Comandos de Desarrollo

### Desarrollo diario
```bash
# Ejecutar en modo debug
flutter run

# Ejecutar con hot reload automático
flutter run --hot

# Ejecutar en dispositivo específico
flutter devices
flutter run -d <device-id>
```

### Análisis y calidad de código
```bash
# Analizar código
flutter analyze

# Formatear código
dart format .

# Ejecutar tests
flutter test

# Cobertura de tests
flutter test --coverage
```

### Construcción para producción
```bash
# Android APK
flutter build apk

# Android App Bundle (recomendado para Play Store)
flutter build appbundle

# iOS (macOS únicamente)
flutter build ios

# Web
flutter build web
```

## 🔧 Configuración del Editor

### VS Code settings.json
```json
{
  "dart.flutterSdkPath": "/path/to/flutter",
  "dart.debugExternalLibraries": false,
  "dart.debugSdkLibraries": false,
  "editor.rulers": [80],
  "editor.tabSize": 2,
  "dart.previewFlutterUiGuides": true,
  "dart.previewFlutterUiGuidesCustomTracking": true
}
```

### Configuración de debug
`.vscode/launch.json`:
```json
{
  "version": "0.2.0",
  "configurations": [
    {
      "name": "Flutter",
      "type": "dart",
      "request": "launch",
      "program": "lib/main.dart"
    },
    {
      "name": "Flutter (Profile)",
      "type": "dart",
      "request": "launch",
      "program": "lib/main.dart",
      "flutterMode": "profile"
    }
  ]
}
```

## 🐛 Solución de Problemas

### Problemas comunes

**"Doctor command":**
```bash
flutter doctor -v
# Resolver cada problema mostrado
```

**Problemas de dependencias:**
```bash
flutter clean
flutter pub get
```

**Problemas de cache:**
```bash
flutter pub cache repair
```

**Problemas de build:**
```bash
flutter clean
cd android && ./gradlew clean && cd ..
flutter pub get
flutter run
```

### Logs de depuración
```bash
# Logs detallados
flutter logs

# Logs de una app específica
flutter logs --device-id <device-id>
```

## 📚 Recursos Adicionales

- [Documentación oficial de Flutter](https://flutter.dev/docs)
- [Dart Language Tour](https://dart.dev/guides/language/language-tour)
- [Flutter Widget Catalog](https://flutter.dev/docs/development/ui/widgets)
- [Provider Package](https://pub.dev/packages/provider)

## 🤝 Obtener Ayuda

Si tienes problemas:
1. Revisa la documentación oficial
2. Busca en [StackOverflow](https://stackoverflow.com/questions/tagged/flutter)
3. Abre un issue en el repositorio
4. Consulta en [Flutter Community](https://flutter.dev/community)