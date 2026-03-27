# Sistema de Gestión de Turnos de Estudiantes

## 1. Descripción del Sistema
Este sistema es una aplicación de consola desarrollada en C++ diseñada para gestionar los turnos de atención de estudiantes. El programa permite registrar nuevos alumnos, atenderlos siguiendo el orden de llegada, visualizar la lista de espera y buscar estudiantes específicos por su nombre.

## 2. Estructura Usada y Justificación
Se implementó una **Lista Doblemente Enlazada** de forma manual, sin utilizar librerías externas (STL). 
- **Justificación**: Esta estructura permite una gestión dinámica de la memoria, permitiendo que la lista crezca o disminuya según sea necesario. Además, al ser doblemente enlazada, permite el recorrido en ambos sentidos (frente a final y viceversa), cumpliendo con el requisito para obtener el punto extra.

## 3. Complejidad de las Operaciones
- **Inserción (Registrar estudiante)**: $O(1)$. Al mantener un puntero al final de la lista, agregar un nuevo estudiante es una operación constante.
- **Eliminación (Atender estudiante)**: $O(1)$. Como se sigue una lógica FIFO (primero en llegar, primero en salir), siempre se elimina el nodo del frente.
- **Búsqueda (Buscar por nombre)**: $O(n)$. En el peor de los casos, se debe recorrer la lista completa para encontrar al estudiante.

## 4. Instrucciones de Compilación y Ejecución
1.  **Compilación**: Use un compilador de C++ (como g++) y ejecute el comando:
    `g++ main.cpp -o sistema`
2.  **Ejecución**: Inicie el programa con el comando:
    `./sistema` (en Linux/Mac) o ejecutando el
