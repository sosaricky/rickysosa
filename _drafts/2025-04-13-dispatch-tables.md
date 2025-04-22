---
layout: default
title: Dispatch tables
date: 2025-04-13
---


Las dispatch tables nos permiten evitar escribir muchos "if" cuando tenemos que evaluar muchas condiciones.
Por ejemplo , supognamos que queremos diseñar una calculadora que según símbolo que le pasemos como parámtro ejecute la operación correspondiente (suma , producto o division)

Primero vamos a realizarlo con "if"
```ruby
class Calculadora

    def realizar_operacion(operacion,operando1,operando2)
```