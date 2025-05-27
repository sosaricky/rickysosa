---
layout: default
title: Dispatch tables
date: 2025-04-13
excerpt: "Reemplazar múltiples ifs usando dispatch tables."
---


Las dispatch tables nos permiten evitar escribir muchos "if" cuando tenemos que evaluar muchas condiciones.
Por ejemplo , supognamos que queremos diseñar una calculadora que según símbolo que le pasemos como parámtro ejecute la operación correspondiente (suma , producto o division)

Primero vamos a realizarlo con "if"
```ruby
class Calculadora
    def self.realizar_operacion(operacion,operando1,operando2)
        if(operacion == '/')
            begin
                operando1 / operando2
            rescue => ZeroDivisionError
                puts 'Segundo operando debe ser distinto de cero'
            end
        end
    end
end

Calculadora.realizar_operacion('/',23,3)
Calculadora.realizar_operacion('/',23,0)

```