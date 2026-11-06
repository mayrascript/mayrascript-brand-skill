# MayraScript Brand Skill

Identidad visual y voz de [MayraScript](https://mayrascript.com/) para interfaces, documentación y workshops. Incluye una guía derivada del sitio público, isotipo, IBM Plex Mono y tokens CSS para claro y oscuro.

La observación inicial es del 6 de noviembre de 2026. Las adaptaciones de accesibilidad y modo claro están identificadas en la guía; no se presentan como un manual oficial previo.

## Instalar en un proyecto

```sh
git clone https://github.com/mayrascript/mayrascript-brand-skill.git
mkdir -p TU_PROYECTO/.agents/skills
cp -R mayrascript-brand-skill/skills/mayrascript-brand TU_PROYECTO/.agents/skills/
```

En un agente compatible, solicita: **“Usa $mayrascript-brand para aplicar el branding a esta interfaz.”** También puedes leer [SKILL.md](skills/mayrascript-brand/SKILL.md) directamente y seguir sus instrucciones.

Para instalarla en Codex para todos tus proyectos, copia la misma carpeta a `~/.codex/skills/mayrascript-brand/`.

## Usar los recursos en una web

Carga `brand-fonts.css` y `brand-tokens.css` antes de tus estilos. Copia los TTF junto a la hoja CSS final y conserva `OFL.txt`. Define estilos de componentes con `var(--ms-bg)`, `var(--ms-text)`, `var(--ms-link)`, etc. El atributo `data-theme="dark"` en `<html>` activa el tema oscuro. El cambio de tema y su persistencia corresponden a la aplicación.

La skill no ejecuta código, no accede a claves y no llama a modelos. Sus instrucciones guían al agente; los activos CSS pueden consumirse directamente en la compilación de la web.

## Referencia en uso

- [Workshop: Tu próximo equipo no es humano](https://mayrascript.github.io/golden-rentals-workshop/)
- [Repositorio del workshop](https://github.com/mayrascript/golden-rentals-workshop)
- [Guía de marca y procedencia](skills/mayrascript-brand/references/brand-guide.md)

Guarda el commit de origen cuando copies la skill a otro proyecto. Para actualizarla, revisa los cambios, sustituye la copia y comprueba ambos temas y tamaños de pantalla.

El isotipo identifica a MayraScript; su inclusión no concede derechos para representar otras marcas. La tipografía incluye su licencia SIL OFL.
