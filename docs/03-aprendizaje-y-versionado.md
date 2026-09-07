# Aprendizaje y versionado

El objetivo no es que la skill crezca sin control.

Queremos que cada mejora tenga una razón clara y que podamos entender por qué se cambió el comportamiento.

## Qué merece documentarse

Un aprendizaje merece registrarse cuando:

- corrige un error que puede repetirse;
- mejora una decisión importante;
- descubre una excepción real;
- cambia el orden óptimo del proceso;
- revela una dependencia o dato necesario;
- evita una acción incorrecta o peligrosa;
- simplifica de forma clara el trabajo.

## Qué no merece convertirse en regla

No debemos añadir una regla nueva por cada caso aislado.

Si algo ocurrió una sola vez y no cambia el diseño general, puede quedarse como nota de prueba.

## Separar comportamiento y aprendizaje

La skill principal debe contener las instrucciones que realmente necesita para trabajar.

Los casos, pruebas y aprendizajes históricos pueden mantenerse fuera para evitar que la definición principal crezca indefinidamente.

La idea es distinguir entre:

- **reglas vigentes**: forman parte de la skill;
- **aprendizajes**: explican por qué existen esas reglas;
- **casos de prueba**: sirven para comprobar que las reglas siguen funcionando.

## Ciclo de mejora

Cada cambio debería seguir este recorrido:

1. Aparece un caso real.
2. Detectamos un problema o mejora.
3. Registramos el aprendizaje.
4. Decidimos si requiere modificar la skill.
5. Actualizamos la skill si procede.
6. Repetimos el caso.
7. Comprobamos que no hemos roto otros comportamientos.

## Versiones

Cuando una modificación cambia de forma relevante el comportamiento, conviene tratarla como una nueva versión.

No necesitamos una gestión compleja al principio. Git ya nos permite saber:

- qué cambió;
- cuándo cambió;
- qué versión funcionaba antes;
- por qué se introdujo una regla.

## Cuando exista el agente desplegado

Los aprendizajes pueden venir de dos sitios:

- pruebas manuales de la skill;
- comportamiento del agente en producción.

Ambos deben alimentar el mismo ciclo de mejora.

La meta es que la skill siga siendo la referencia funcional del comportamiento, aunque después exista código desplegado.
