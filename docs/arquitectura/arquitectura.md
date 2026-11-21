# Arquitectura de Android-Edge Sandbox

## 1. Visión general

El proyecto utiliza Linux como sistema anfitrión y Waydroid
como entorno de ejecución de Android mediante contenedores.

## 2. Capas del sistema

### Equipo físico
Computadora con arquitectura x86_64.

### Virtualización
VirtualBox ejecutándose sobre Windows.

### Sistema anfitrión
Distribución Linux de 64 bits, prevista inicialmente:
Debian.

### Entorno Android
Waydroid, encargado de ejecutar los servicios y procesos
necesarios de Android.

### Integración gráfica
Wayland, para la comunicación entre el entorno gráfico
Linux y la interfaz Android.

## 3. Componentes principales

- Kernel Linux.
- Binder IPC.
- Ashmem o alternativa compatible que se verifique.
- Wayland.
- zRAM.
- cgroups v2.
- lmkd.
- Seccomp-BPF.
- AppArmor.

## 4. Seguridad y auditoría

Se estudiarán los mecanismos de aislamiento y control,
la observación de llamadas al sistema y las comunicaciones
mediante sockets UNIX.

## 5. Gestión de recursos

Se evaluará el consumo de CPU y memoria, incluyendo
pruebas controladas de presión de memoria.

## 6. Consideraciones técnicas

La compatibilidad gráfica de Waydroid dentro de VirtualBox
debe comprobarse experimentalmente.

Los componentes y mecanismos se documentarán según su
compatibilidad real con la distribución y el kernel elegidos.

## 7. Estado

Documento inicial. Arquitectura pendiente de validación
durante la implementación.
