# EvaluacionHito2_SIS_12992520_SamuelVillca
Desarrollo un sistema en consola para la gestión de turnos de atención de estudiantes.

# Sistema de Gestión de Turnos de Estudiantes

## [cite_start]1. Descripción del Sistema [cite: 41]
Esra es una aplicación de consola desarrollada en C++ para gestionar turnos de atención en orden de llegada. Permite registrar estudiantes, atenderlos, buscarlos por nombre y visualizar la lista de espera.

## [cite_start]2. Estructura Usada y Justificación [cite: 42]
[cite_start]Se implementó una **Lista Doblemente Enlazada** manual[cite: 35, 37]. 
- [cite_start]**Justificación**: Se eligió esta estructura porque permite un manejo dinámico de la memoria (la lista crece según llegan alumnos) y, al ser doblemente enlazada, permite recorridos bidireccionales (hacia adelante y hacia atrás), cumpliendo con el requisito de punto extra[cite: 68].

## [cite_start]3. Complejidad de las Operaciones [cite: 43]
| Operación | Complejidad | Descripción |
| :--- | :--- | :--- |
| **Inserción (Registrar)** | $O(1)$ | Al tener un puntero al `final`, la inserción es inmediata. |
| **Eliminación (Atender)** | $O(1)$ | Al eliminar siempre del `frente`, la operación es constante. |
| **Búsqueda** | $O(n)$ | En el peor de los casos, se debe recorrer toda la lista. |

## [cite_start]4. Instrucciones de Compilación y Ejecución [cite: 44]
1. Asegúrese de tener un compilador de C++ (como G++).
2. Compile el archivo con: `g++ main.cpp -o sistema`
3. Ejecute con: `./sistema` (en Linux/Mac) o `sistema.exe` (en Windows).

## 5. Datos del Estudiante
- **Nombre**: [Tu Nombre Completo]
- [cite_start]**Repositorio**: examen-estructuras-datos-[tu-nombre-apellido]
