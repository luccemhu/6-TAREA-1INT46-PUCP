# [6-TAREA-1INT46-PUCP](https://luccemhu.github.io/6-TAREA-1INT46-PUCP/)

# **Rock, Paper, Scissors Simulation with OOP**

Repositorio: https://github.com/luccemhu/6-TAREA-1INT46-PUCP

Github Pages: https://luccemhu.github.io/6-TAREA-1INT46-PUCP/

## **Descripción General**
Este repositorio implementa un simulador del clásico juego "Piedra, Papel o Tijera" utilizando conceptos de **Programación Orientada a Objetos (OOP)**. Los jugadores compiten en varias rondas, y el programa declara al ganador basado en el puntaje acumulado.

---

## **Estructura del Proyecto**

### **1. Clases**
#### **`Player`**
- Representa un jugador básico.
- **Atributos**:
  - `name`: Nombre del jugador.
  - `score`: Puntaje acumulado.
- **Métodos**:
  - `increase_score(value)`: Incrementa el puntaje del jugador.

#### **`PlayerBetter`**
- Hereda de `Player`.
- **Atributos adicionales**:
  - `strategy`: Última estrategia elegida.
- **Métodos adicionales**:
  - `get_strategy()`: Elige una estrategia aleatoria.

#### **`Game`**
- Maneja el flujo del juego.
- **Atributos**:
  - `players`: Lista de jugadores.
- **Métodos**:
  - `play_round()`: Enfrenta a todos los pares de jugadores en una ronda.
  - `play_game(rounds)`: Ejecuta múltiples rondas.
  - `declare_winner()`: Determina el ganador basado en el puntaje.
  - `show_results()`: Muestra los puntajes finales.

---

### **2. Configuración**
- **Jugadores**: Incluye nombres como `'Gian'`, `'Lucho'`, `'Joel'`, `'Chavi'` y reconocidos politólogos latinoamericanos.
- **Estrategias**: `'Rock'`, `'Paper'`, `'Scissors'`.
- **Reglas del Juego**:
```python
payoff = {
    ('Rock', 'Paper'): (0, 1),
    ('Paper', 'Rock'): (1, 0),
    ('Rock', 'Scissors'): (1, 0),
    ('Scissors', 'Rock'): (0, 1),
    ('Paper', 'Scissors'): (0, 1),
    ('Scissors', 'Paper'): (1, 0),
    ('Rock', 'Rock'): (0, 0),
    ('Paper', 'Paper'): (0, 0),
    ('Scissors', 'Scissors'): (0, 0)
}
