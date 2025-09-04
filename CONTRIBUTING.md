# Contribuir a TimerRubik

¡Gracias por tu interés en contribuir a TimerRubik! Este documento te guía sobre cómo contribuir al proyecto.

## 🚀 Cómo contribuir

### Reportar bugs

1. Verifica que el bug no haya sido reportado anteriormente en los [issues](https://github.com/Tend0Dev/TimerRubik/issues)
2. Crea un nuevo issue con:
   - Título descriptivo
   - Descripción detallada del problema
   - Pasos para reproducir el bug
   - Comportamiento esperado vs comportamiento actual
   - Capturas de pantalla (si aplica)
   - Información del dispositivo/plataforma

### Sugerir mejoras

1. Abre un issue con el tag "enhancement"
2. Describe claramente la mejora propuesta
3. Explica por qué sería útil para los usuarios
4. Considera incluir mockups o diagramas si es apropiado

### Contribuir código

1. **Fork** el repositorio
2. **Clona** tu fork localmente:
   ```bash
   git clone https://github.com/TU_USUARIO/TimerRubik.git
   cd TimerRubik
   ```

3. **Crea una rama** para tu contribución:
   ```bash
   git checkout -b feature/descripcion-corta
   # o
   git checkout -b fix/descripcion-del-bug
   ```

4. **Configura el entorno de desarrollo**:
   ```bash
   flutter pub get
   flutter analyze
   flutter test
   ```

5. **Realiza tus cambios**:
   - Mantén el código limpio y bien documentado
   - Sigue las convenciones de Flutter/Dart
   - Agrega tests si es apropiado
   - Actualiza documentación si es necesario

6. **Verifica tu código**:
   ```bash
   flutter analyze
   flutter test
   flutter build apk --debug  # Para verificar que compila
   ```

7. **Commit tus cambios**:
   ```bash
   git add .
   git commit -m "Descripción clara de los cambios"
   ```

8. **Push a tu fork**:
   ```bash
   git push origin feature/descripcion-corta
   ```

9. **Crea un Pull Request**:
   - Ve a GitHub y crea un PR desde tu rama
   - Describe claramente qué cambios realizaste
   - Referencia issues relacionados si aplica

## 📝 Estándares de código

### Convenciones de nomenclatura

- **Archivos**: snake_case (ej: `rubik_timer.dart`)
- **Clases**: PascalCase (ej: `RubikTimer`)
- **Variables y funciones**: camelCase (ej: `startTimer()`)
- **Constantes**: SCREAMING_SNAKE_CASE (ej: `DEFAULT_TIME`)

### Estructura de archivos

- Mantén los archivos organizados según la estructura existente
- Un archivo por clase principal
- Agrupa funcionalidades relacionadas en carpetas

### Comentarios

- Usa comentarios en español (idioma del proyecto)
- Documenta funciones complejas
- Explica el "por qué", no solo el "qué"

### Tests

- Agrega tests para nueva funcionalidad
- Mantén los tests existentes funcionando
- Usa nombres descriptivos para los tests

## 🎯 Áreas donde necesitamos ayuda

- **Algoritmos**: Agregar más algoritmos (ZBLL, COLL, etc.)
- **Estadísticas**: Implementar promedios de 5, 12, 100
- **UI/UX**: Mejorar la interfaz de usuario
- **Performance**: Optimizar el rendimiento del timer
- **Tests**: Agregar más cobertura de tests
- **Documentación**: Mejorar y ampliar la documentación
- **Localización**: Soporte para más idiomas

## 🔄 Proceso de revisión

1. Todos los PRs serán revisados por los mantenedores
2. Pueden solicitar cambios o aclaraciones
3. Una vez aprobado, el PR será merged
4. Se agradece la paciencia durante el proceso de revisión

## 📞 Contacto

Si tienes preguntas sobre cómo contribuir:
- Abre un issue con el tag "question"
- Contacta a los mantenedores

¡Gracias por ayudar a hacer TimerRubik mejor! 🎲⏱️