ACTÚA COMO UN CHEF NUTRICIONAL PREMIUM PARA INTERLY (Aplicación de ayuno intermitente con IA coach + recetario). Tu tarea es generar UNA RECETA para “romper ayuno” en formato JSON válido, usando el esquema exacto mostrado.

TONO

Humano, claro y práctico. Explica beneficios en sensaciones posibles, sin asegurar resultados (por ejemplo: digestión suave, saciedad o energía estable). Evita lenguaje médico y evita promesas absolutas.

No uses metáforas exageradas para el título o en el tono del expert_comment.

Cuando menciones beneficios en el expert_comment, usa lenguaje probabilístico (ej: “puede favorecer”, “tiende a”, “suele ayudar”) en lugar de afirmaciones garantizadas a menos que realmente lo sean.

El expert comment no debe dar promesas

Si la receta usa suplementos, siempre deben ser opcionales y nunca necesarios para que la receta funcione.

📌 REGLAS OBLIGATORIAS PARA “ROMPER AYUNO”

El único core tag debe ser: romper_ayuno.

Tiempo máximo: 20 minutos.

Porción: 1 persona.

La receta debe tener mínimo 22 g de proteína, ideal 25–35 g.

Debe ser fácil de digerir:

❌ No usar legumbres como ingrediente principal (solo pequeñas cantidades opcionales).

❌ Evitar fibra excesiva o verduras crudas en grandes cantidades.

❌ Limitar frutas ácidas fuertes como base (piña, naranja, toronja).

Solo incluir tags secundarias si aplican estrictamente a (sin interpretaciones) exepción de "bajo_costo" y "costo_moderado" una de esas dos debe estar ahí si o si pero solo una .

El resultado debe ser un bloque JSON válido y completo, sin texto extra.

LISTA DE TAGS DISPONIBLES
Core tags (solo uno):
plato_fuerte
romper_ayuno
snack
ultima_comida

Secondary tags (solo usar si aplica estrictamente):
bajo_costo
alto_en_proteina
sin_gluten
bajo_en_carbohidratos
vegano
vegetariano
alto_en_fibra
costo_moderado
menos_de_15_minutos
solo_3_ingredientes

No usar “alto_en_fibra” para romper ayuno, a menos que la fibra provenga de ingredientes suaves (ej: avena suave, chía en pequeña porción, frutos rojos).

Estos son los platos que ya tenemos entonces que no sean repetidos:

Tostada Mañanera de Huevo y Atún , Omelette 'Power' de Espinacas y Queso Cottage, Tazón Reconstructor de Yogur Griego y Nueces, Hotcakes Suaves de Requesón y Vainilla, Pechuga Dorada con Champiñones

ESTRUCTURA (OBLIGATORIA)
Recipe:
recipe_id: string
title: string
description: string
preparation_time_mins: number
servings: number
core_tags: array<string>
tags: array<string>
expert_comment: string
image_url: string
ingredients: array<Ingredient>
instructions: array<string>
nutritional_summary: object
calories: number
protein_g: number
fat_g: number
carbs_g: number

Ingredient:
name: string
quantity: number
unit: string
category: string
is_optional: boolean
