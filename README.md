# Administrador de pacientes veterinarios

Aplicación web para registrar y administrar pacientes y sus citas en una clínica veterinaria. Está construida con TypeScript, Vite y Tailwind CSS.

## Requisitos

- Node.js 18 o posterior
- npm

## Instalación y ejecución

Clona el repositorio y entra en la carpeta del proyecto:

```bash
git clone https://github.com/MarioGarcia08/Gestion-Veterinaria.git
cd Gestion-Veterinaria
```

Instala las dependencias y arranca el servidor de desarrollo:

```bash
npm install
npm run dev
```

Vite mostrará en la terminal la dirección local para abrir la aplicación en el navegador.

## Comandos disponibles

| Comando | Descripción |
| --- | --- |
| `npm run dev` | Inicia el servidor de desarrollo. |
| `npm run build` | Comprueba los tipos de TypeScript y genera la versión de producción en `dist/`. |
| `npm run preview` | Sirve localmente la versión de producción generada por `npm run build`. |

Para probar la versión de producción:

```bash
npm run build
npm run preview
```

## Funcionalidades

- Registrar pacientes con nombre, propietario, correo electrónico, fecha y síntomas.
- Consultar los pacientes registrados durante la sesión.
- Editar o eliminar registros.
- Validar que los campos estén completos antes de guardar.

> **Importante:** los registros se guardan únicamente en la memoria de la aplicación. Se pierden al recargar o cerrar la página; el proyecto no incluye base de datos ni almacenamiento persistente.

## Estructura del proyecto

```text
├── index.html                 # Página y formulario de la aplicación
├── public/                    # Recursos estáticos
├── src/
│   ├── app.ts                 # Punto de entrada y eventos del formulario
│   ├── classes/
│   │   ├── AdminCitas.ts      # Gestión y visualización de registros
│   │   └── Notificacion.ts    # Mensajes de validación y confirmación
│   ├── funciones.ts           # Registro, edición y validación
│   ├── selectores.ts          # Selectores del DOM
│   ├── style.css              # Estilos y directivas de Tailwind CSS
│   ├── types.ts               # Tipos de TypeScript
│   └── variables.ts           # Estado del formulario
├── package.json               # Dependencias y comandos npm
└── tsconfig.json              # Configuración de TypeScript
```
