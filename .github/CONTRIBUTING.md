# 🤝 Guía de Contribución

¡Gracias por tu interés en contribuir a **Smart Track**! Este documento describe el proceso y las convenciones que seguimos para mantener el proyecto ordenado y colaborativo.

---

## 📋 Tabla de contenidos

- [🤝 Guía de Contribución](#-guía-de-contribución)
  - [📋 Tabla de contenidos](#-tabla-de-contenidos)
  - [📜 Código de conducta](#-código-de-conducta)
  - [🙌 ¿Cómo puedo contribuir?](#-cómo-puedo-contribuir)
  - [🌿 Flujo de trabajo con Git](#-flujo-de-trabajo-con-git)
  - [✍️ Convenciones de commits](#️-convenciones-de-commits)
    - [Tipos permitidos](#tipos-permitidos)
    - [Ejemplos](#ejemplos)
  - [🌿 Convenciones de ramas](#-convenciones-de-ramas)
  - [🔀 Pull Requests](#-pull-requests)
  - [🐛 Reportar bugs](#-reportar-bugs)
  - [💡 Proponer mejoras](#-proponer-mejoras)
  - [🎨 Estilo de código](#-estilo-de-código)

---

## 📜 Código de conducta

Se espera que todos los colaboradores mantengan un entorno respetuoso e inclusivo. Cualquier comportamiento inapropiado debe reportarse a los mantenedores del proyecto.

---

## 🙌 ¿Cómo puedo contribuir?

- Reportando bugs mediante la plantilla **Bug Report**
- Proponiendo nuevas funcionalidades o endpoints mediante las plantillas de issues correspondientes
- Revisando y comentando Pull Requests abiertos
- Mejorando la documentación
- Escribiendo o mejorando tests

---

## 🌿 Flujo de trabajo con Git

Seguimos un flujo basado en **feature branches**:

1. Asegúrate de partir siempre desde `main` actualizado:
   ```bash
   git checkout main
   git pull origin main
   ```

2. Crea una nueva rama con la convención establecida (ver [Convenciones de ramas](#convenciones-de-ramas)):
   ```bash
   git checkout -b feat/nombre-descriptivo
   ```

3. Realiza tus cambios en commits atómicos y bien descritos.

4. Sube tu rama y abre un Pull Request hacia `main`.

---

## ✍️ Convenciones de commits

Usamos **Conventional Commits**. El formato es:

```
<tipo>(<ámbito>): <descripción corta>
```

### Tipos permitidos

| Tipo       | Descripción                                               |
|------------|-----------------------------------------------------------|
| `feat`     | Nueva funcionalidad                                       |
| `fix`      | Corrección de un bug                                      |
| `docs`     | Cambios en documentación                                  |
| `style`    | Cambios de formato (sin afectar lógica)                   |
| `refactor` | Refactoring de código sin nueva funcionalidad ni bug fix  |
| `test`     | Añadir o corregir tests                                   |
| `chore`    | Tareas de mantenimiento, dependencias, configuración      |
| `perf`     | Mejoras de rendimiento                                    |
| `ci`       | Cambios en configuración de CI/CD                         |
| `db`       | Cambios en base de datos (migraciones, esquemas)          |

### Ejemplos

```
feat(api): añadir endpoint de autenticación con JWT
fix(users): corregir validación de email duplicado
db(orders): añadir índice en campo created_at
docs: actualizar guía de instalación
```

---

## 🌿 Convenciones de ramas

| Prefijo        | Uso                                        | Ejemplo                          |
|----------------|--------------------------------------------|----------------------------------|
| `feat/`        | Nueva funcionalidad                        | `feat/login-oauth`               |
| `fix/`         | Corrección de bug                          | `fix/token-expiration`           |
| `refactor/`    | Refactoring                                | `refactor/user-service`          |
| `docs/`        | Documentación                              | `docs/api-readme`                |
| `test/`        | Tests                                      | `test/auth-unit-tests`           |
| `chore/`       | Mantenimiento                              | `chore/update-dependencies`      |
| `db/`          | Cambios en base de datos                   | `db/add-phone-column`            |
| `hotfix/`      | Corrección urgente en producción           | `hotfix/critical-null-pointer`   |

---

## 🔀 Pull Requests

- Rellena completamente la plantilla del PR.
- Asegúrate de que todos los checks de CI pasan antes de solicitar revisión.
- Asocia siempre el PR a su issue correspondiente con `Closes #<número>`.
- Solicita al menos **1 aprobación** antes de hacer merge.
- No hagas merge de tu propio PR salvo casos excepcionales acordados con el equipo.
- Usa **Squash and Merge** para mantener un historial limpio en `main`.

---

## 🐛 Reportar bugs

Usa la plantilla **Bug Report** en la sección de Issues. Incluye siempre:

- Pasos para reproducir el error
- Comportamiento esperado vs. actual
- Logs o stack trace si están disponibles
- Entorno donde ocurre (producción, staging, local)

---

## 💡 Proponer mejoras

Usa la plantilla de issues correspondiente según el tipo de propuesta:

- **API Proposal** → para nuevos endpoints o cambios de contrato
- **BD Update** → para cambios en el esquema de base de datos
- **Technical Question** → para dudas técnicas o de arquitectura

---

## 🎨 Estilo de código

- Sigue las reglas del linter configurado en el proyecto (ESLint / Prettier / u otros según el repositorio).
- Ejecuta el formateador antes de hacer commit.
- Escribe nombres de variables y funciones en **inglés**.
- Los comentarios y mensajes de commit pueden escribirse en **español o inglés**, de forma consistente por proyecto.

---

Si tienes cualquier duda, abre una issue con la plantilla **Technical Question** o contacta directamente con los mantenedores del proyecto. ¡Tu contribución es bienvenida! 🚀
