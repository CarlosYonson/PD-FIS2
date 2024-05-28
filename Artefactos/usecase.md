# Caso de Uso: Establecer Metas Nutricionales

## Objetivo
Permitir que el nutricionista establezca y gestione metas nutricionales personalizadas para cada paciente utilizando el sistema basado en la nube.

## Actores
- **Nutricionista** (Usuario Principal)
- **Almacenamiento en la Nube**

## Flujo Principal de Eventos
1. El nutricionista inicia sesión en el software de cálculo nutricional en la nube.
2. Selecciona la opción "Establecer Metas Nutricionales" del menú principal.
3. Elige un paciente específico para establecer metas nutricionales.
4. El sistema recupera los datos nutricionales actuales y el historial del paciente desde la nube.
5. El nutricionista define metas nutricionales personalizadas (ingesta calórica diaria, distribución de macronutrientes, peso objetivo).
6. El sistema almacena las metas en la nube, asociadas con el paciente.

## Flujos Alternativos de Eventos
- Si se intentan establecer metas poco realistas, el sistema advierte y sugiere objetivos más alcanzables.
- Si hay problemas al guardar, el sistema informa al nutricionista y recomienda verificar la conexión a internet.

## Precondiciones
- El nutricionista debe tener acceso a internet.
- El software de cálculo nutricional debe estar operativo.

## Postcondiciones
- Las metas nutricionales se establecen y almacenan exitosamente en la nube para el paciente.
