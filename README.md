# Práctica 3 - Final

Basado en la práctica FPOO-Practica-3-herencia-2, se deberá actualizar el sistema con los siguiente requerimientos.

**Título: Sistema de Gestión de Flota para una Empresa de Transporte Multimodal**

**Descripción:**
Se requiere desarrollar un sistema de gestión de flota para una empresa de transporte que opera con vehículos terrestres y marítimos. La empresa cuenta con tres tipos de vehículos terrestres: coches, camiones y motocicletas, así como varios tipos de buques para el transporte marítimo. El sistema debe ser implementado como una aplicación de línea de comandos y debe cumplir con los siguientes requerimientos:

1. **Clases de Vehículos Terrestres:**
    - `Coche`: Representa un coche con un número de identificación único, capacidad de pasajeros y cálculo de costo de viaje.
    - `Camion`: Representa un camión con un número de identificación único, capacidad de carga en toneladas y cálculo de costo de viaje.
    - `Motocicleta`: Representa una motocicleta con un número de identificación único, cilindrada y cálculo de costo de viaje.
    - Subclases de `Camion`:
        - `CamionPlataformaAbierta`
        - `CamionConLona`
        - `CamionFrigorifico` (con diferentes tipos: refrigerado, congelado, etc.)
        - `CamionCisterna` (para transportar líquidos: físico-químicos, tóxicos, etc.)
        - `CamionCerrado`
        - `CamionPortacoches`
        - `CamionJaula`
        - `CamionContenedor`

2. **Clases de Vehículos Marítimos:**
    - `BuqueDeCarga`: Representa un buque de carga con un número de identificación único y capacidad de carga en toneladas.
    - Subclases de `BuqueDeCarga`:
        - `Portacontenedores`
        - `BuqueGranelero` (para cargas a granel)
        - `BuqueRoRo` (Roll on – Roll off o de cargamento rodado)
        - `Petrolero`
        - `BuqueFrigorifico`
        - `Gasero`
        - `BuqueQuimico` (para cargas químicas)
        - `BuqueDeGanado`

3. **Usuarios:**
    - `Administrador`: Puede agregar, editar y eliminar vehículos y usuarios.
    - `Gerente`: Puede ver estadísticas, generar reportes y administrar la flota.
    - `UsuarioDeCaja`: Puede registrar transacciones de pago y generar facturas.

4. **Cálculo del Costo del Viaje:**
    - Para cada vehículo, se debe calcular el costo del viaje considerando la distancia y el consumo de combustible por kilómetro. El costo se calculará como: `(kilómetros * precio de combustible) + 15% del total por depreciación del vehículo`. Se considera que cada vehículo utiliza un tipo diferente de combustible.

5. **Búsqueda de Vehículos:**
    - Los clientes pueden buscar vehículos por número de identificación o por capacidad de carga.

6. **Requerimientos No Funcionales:**
    - **Usabilidad**: La interfaz de línea de comandos debe ser intuitiva y fácil de usar.
    - **Precisión**: La información almacenada debe ser precisa y confiable.
    - **Disponibilidad**: El sistema debe estar disponible durante el horario de operación de la empresa.
    - **Seguridad**: La información debe estar protegida contra accesos no autorizados.
    - **Escalabilidad**: El sistema debe manejar un alto volumen de transacciones.
    - **Mantenibilidad**: El sistema debe ser fácil de mantener y actualizar.
    - **Rendimiento**: El sistema debe responder eficientemente incluso bajo carga.

Este sistema permitirá a la empresa gestionar su flota multimodal de manera eficiente y brindar un servicio de transporte confiable a sus clientes tanto en tierra como en el mar.
