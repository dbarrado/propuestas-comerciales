# Propuestas comerciales — skill para Claude

Skill que arma **propuestas comerciales en Word** con la marca, los precios y los servicios de tu empresa. Sirve para cualquier rubro y distingue si el cliente es una **empresa (B2B)** o un **particular (B2C)**.

Aplica:

- **Busca primero los datos de tu empresa** (quién es, marca, tarifario, consulta del cliente) y **pregunta lo que falta** en vez de inventarlo.
- **Cada número sale de un archivo**: usa solo precios vigentes y avisa si dos documentos se contradicen.
- **Lo que falta se marca «por confirmar»**: fechas, plazos, validez, forma de pago, descuentos.
- **Trato según el cliente**: a una empresa, dirigida a quien consultó con su cargo y con condiciones explícitas; a un particular, por su nombre y en palabras simples.
- **Revisión antes de entregar**: rehace las cuentas, separa lo mensual del pago único y comprueba la marca.
- **Se adapta a tu proyecto**: la primera vez ofrece guardar en las instrucciones del proyecto dónde están tus datos, para no volver a preguntar.

La propuesta no se envía sola: la manda una persona después de revisarla.

## Cuándo se activa

Cuando le pedís a Claude cosas como: *"armá la propuesta para este cliente"*, *"presupuesto formal en Word"*, *"propuesta comercial para la consulta que llegó"*.

## Instalación

Una skill es una carpeta con un `SKILL.md` adentro.

### Opción A — desde la app de Claude (Personalizar)

1. Descargá [`propuestas-comerciales.zip`](https://github.com/dbarrado/propuestas-comerciales/releases/latest/download/propuestas-comerciales.zip).
2. En Claude, entrá a **Personalizar → Skills**, tocá **+** y elegí **subir una skill**.
3. Elegí el ZIP que descargaste, sin descomprimirlo.

### Opción B — pedírselo al agente

En una sesión de Claude Code (o Codex) con la carpeta de tu proyecto, pegá:

> Instalá como skill de este proyecto la skill de https://github.com/dbarrado/propuestas-comerciales

### Opción C — a mano

Copiá la carpeta [`propuestas-comerciales`](propuestas-comerciales) dentro de la carpeta de skills:

- **Por proyecto:** `<tu proyecto>/.claude/skills/propuestas-comerciales/SKILL.md`
- **Para todos tus proyectos:** `~/.claude/skills/propuestas-comerciales/SKILL.md` (en Windows: `%USERPROFILE%\.claude\skills\`)

## Verificación

Abrí una sesión nueva y pedí *"armá una propuesta para [cliente]"*. Antes de escribir, la skill te dice si el cliente es empresa o particular y te pregunta lo que no encuentra en tu carpeta.

## Licencia

MIT. Material del curso «IA para profesionales» de Strategic IA.
