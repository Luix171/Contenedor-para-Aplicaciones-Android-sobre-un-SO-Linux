# Android-Edge Sandbox

Entorno seguro y contenedor de pruebas para la ejecución de
aplicaciones Android sobre un sistema operativo Linux.

## Propósito

Diseñar, configurar y documentar un entorno basado en Linux
x86_64 que permita ejecutar Android dentro de un contenedor,
estudiando el aislamiento, la seguridad y la administración
de recursos del sistema anfitrión.

## Arquitectura prevista

- Sistema anfitrión: Linux x86_64.
- Entorno Android: Waydroid.
- Integración gráfica: Wayland.
- Comunicación entre procesos: Binder IPC.
- Gestión de memoria: zRAM, cgroups v2 y lmkd.
- Seguridad: Seccomp-BPF y AppArmor.
- Auditoría: observación de syscalls y sockets UNIX.

## Entorno de desarrollo

- Sistema de trabajo: Windows 10.
- Virtualización: VirtualBox.
- Distribución Linux prevista: Debian de 64 bits.

## Estructura

- docs/: documentación técnica y académica.
- scripts/: automatización y configuración.
- config/: archivos de configuración.
- tests/: pruebas de funcionamiento.

## Estado del proyecto

Fase 1: Fundación, arranque y kernel.

## Equipo

Proyecto académico de Sistemas Operativos.
