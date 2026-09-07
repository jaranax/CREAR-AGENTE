# Flujo de trabajo

Este documento explica la dinámica que queremos seguir cada vez que detectemos una tarea que podría convertirse en un agente.

## 1. Detectar una tarea útil

La pregunta inicial no es "¿qué agente puedo crear?" sino:

**¿Qué tarea repetitiva, concreta y valiosa queremos resolver?**

La tarea debe poder describirse con claridad.

## 2. Definir el comportamiento esperado

Antes de construir nada, dejamos claro:

- qué información recibe;
- qué debe hacer;
- qué resultado debe entregar;
- qué decisiones puede tomar;
- qué herramientas necesita;
- qué situaciones requieren detenerse o pedir revisión.

## 3. Crear la primera skill

La skill es nuestro laboratorio.

Aquí convertimos el proceso en instrucciones ejecutables dentro de ChatGPT.

No buscamos que la primera versión sea perfecta. Buscamos poder empezar a probar.

## 4. Ejecutar casos reales

Probamos la skill con trabajo real.

Cada prueba debe responder a una pregunta sencilla:

**¿Ha hecho lo que esperábamos?**

Si la respuesta es no, debemos identificar por qué.

## 5. Registrar aprendizajes

No todo error merece convertirse en una regla nueva.

Documentamos solo aquello que realmente mejora el comportamiento futuro:

- errores repetibles;
- excepciones importantes;
- decisiones que deben seguir siempre el mismo criterio;
- nueva información necesaria;
- pasos que sobran;
- controles que faltan.

## 6. Actualizar la skill

El aprendizaje se incorpora donde corresponda.

Después volvemos a probar.

Este ciclo puede repetirse muchas veces:

**Skill → caso real → aprendizaje → modificación → nuevo caso real**

## 7. Decidir si merece convertirse en agente

Cuando la skill ya resuelve bien el proceso, decidimos si tiene sentido sacarla de ChatGPT.

Si solo la utilizamos ocasionalmente de forma manual, quizá no haga falta crear un agente.

Si necesitamos que trabaje solo, por horario, por eventos o conectado permanentemente a otros sistemas, sí empieza a tener sentido.

## 8. Crear la especificación del agente

La skill validada deja de ser solo un prompt y pasa a convertirse en la referencia funcional del agente.

A partir de ella se documentan también aspectos que en la fase de pruebas podían ser secundarios:

- autenticación;
- conectores;
- memoria;
- almacenamiento;
- logs;
- tratamiento de errores;
- reintentos;
- permisos;
- eventos que lo activan.

## 9. Generar y desplegar

La intención es utilizar herramientas de desarrollo, como Codex, para convertir esa especificación en código desplegable.

La infraestructura prevista inicialmente es Cloudflare.

## 10. Continuar aprendiendo

Una vez desplegado, empiezan a aparecer casos que no vimos durante las pruebas.

Estos casos deben alimentar de nuevo la documentación y las siguientes versiones.

El sistema nunca se considera cerrado.

## Resumen operativo

1. Encontrar una tarea.
2. Crear una skill mínima.
3. Probar con trabajo real.
4. Documentar aprendizajes.
5. Mejorar la skill.
6. Repetir hasta conseguir consistencia.
7. Decidir si necesita autonomía.
8. Especificar el agente.
9. Generar código.
10. Desplegar.
11. Aprender del uso real.
12. Mejorar la siguiente versión.
