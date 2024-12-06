# Pokédex en Python

Este es un proyecto que utiliza Python y la **PokeAPI** para crear una Pokédex interactiva. El programa permite al usuario buscar información sobre un Pokémon por su nombre, mostrar sus estadísticas principales y guardar estos datos en un archivo `.json`.

## Características

1. **Consumo de la API de PokeAPI:**  
   El programa consume datos directamente de [PokeAPI](https://pokeapi.co/), obteniendo información actualizada de los Pokémon.

2. **Validación de Status Codes:**  
   Si el Pokémon ingresado no existe, el programa maneja el error mostrando un mensaje amigable.

3. **Despliegue de Información:**  
   Muestra estadísticas principales como:
   - Imagen del Pokémon.
   - Peso (convertido a kilogramos).
   - Altura (convertida a metros).
   - Movimientos.
   - Habilidades.
   - Tipos.

4. **Guardado en Archivo .json:**  
   La información del Pokémon, incluida su imagen frontal, se guarda en un archivo `.json` en una carpeta llamada `pokedex` que se genera automáticamente en el escritorio del usuario.

5. **Estructura del Código:**  
   El código está organizado en funciones bien definidas y comentado para facilitar su comprensión.

---

## Requisitos

Para ejecutar este proyecto, necesitarás:

- **Python 3.8 o superior.**
- Librerías adicionales:
  - `requests`

## Instalación de librerías

Puedes instalar la librería requerida con el siguiente comando:

```bash
pip install requests

## Uso
1 Clona este repositorio en tu máquina local: git clone https://github.com/tuusuario/pokedex.git

2 Navega al directorio del proyecto: cd pokedex

3 Ejecuta el programa: python pokedex.py

Introduce el nombre de un Pokémon cuando se te solicite. Por ejemplo:
Introduce el nombre del Pokémon: pikachu

Si el Pokémon existe, verás la información en la consola y se generará un archivo .json en la carpeta pokedex en tu escritorio.

## Ejemplo de Salida

Imagen: https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/25.png
Peso: 6.0 kg
Altura: 0.4 m
Movimientos: quick-attack, thunderbolt, iron-tail, etc.
Habilidades: static, lightning-rod
Tipos: electric

## Archivo JSON Generado:
{
    "imagen": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/25.png",
    "peso": 6.0,
    "altura": 0.4,
    "movimientos": ["quick-attack", "thunderbolt", "iron-tail", "..."],
    "habilidades": ["static", "lightning-rod"],
    "tipos": ["electric"]
}

## Lo que Aprendí:

Cómo consumir datos de una API RESTful usando Python y la librería requests.
Manejar errores HTTP, como el código 404, de manera efectiva.
Crear y guardar archivos .json con Python.
Organizar mi código en funciones para mejorar su claridad y mantenimiento.
Usar la biblioteca os para crear carpetas y manejar rutas en diferentes sistemas operativos.
Subir un proyecto a GitHub, incluyendo la creación de un archivo README.md detallado.