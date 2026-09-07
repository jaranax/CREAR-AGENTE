# Checklist para crear una nueva skill

Usa esta plantilla antes de empezar a probar una nueva automatización.

## 1. Problema

- ¿Qué tarea concreta queremos resolver?
- ¿Quién la realiza hoy?
- ¿Qué parte consume tiempo o genera errores?

## 2. Objetivo

- ¿Qué resultado debe conseguir la skill?
- ¿Cómo sabremos que lo ha hecho bien?

## 3. Entradas

- ¿Qué información necesita recibir?
- ¿De dónde sale esa información?

## 4. Acciones

- ¿Qué pasos debe ejecutar?
- ¿Qué decisiones debe tomar?
- ¿En qué orden?

## 5. Herramientas

- ¿Necesita Drive, Sheets, Gmail, APIs, base de datos u otros conectores?
- ¿Qué permisos necesita realmente?

## 6. Salidas

- ¿Qué debe entregar?
- ¿Dónde debe guardar o registrar el resultado?

## 7. Errores y límites

- ¿Qué datos pueden faltar?
- ¿Qué situaciones deben detener el proceso?
- ¿Cuándo necesita revisión humana?

## 8. Casos de prueba

Preparar casos que cubran:

- un caso normal;
- un caso con datos incompletos;
- una excepción conocida;
- un caso que no debería ejecutar.

## 9. Aprendizajes

Después de cada prueba:

- ¿qué ha fallado?;
- ¿por qué?;
- ¿es un caso aislado o una regla general?;
- ¿hay que modificar la skill?;
- ¿hay que añadir un nuevo caso de prueba?

## 10. Decisión final

Antes de crear un agente independiente, responder:

- ¿la skill funciona de forma consistente?;
- ¿el proceso está suficientemente definido?;
- ¿necesitamos que trabaje de forma autónoma?;
- ¿qué debe persistir fuera de ChatGPT?;
- ¿qué conectores necesitará en producción?;

Si estas respuestas están claras, podemos pasar a la especificación del agente.
