# Skills de Ami

Skills para que un agente de programación construya con
[Ami](https://amiagente.com). Están en el formato abierto de
[Agent Skills](https://agentskills.io), el que leen Claude Code, Codex, Cursor,
Antigravity y otros.

| Skill | Para qué |
| --- | --- |
| [`ami-storefront`](skills/ami-storefront) | Construir o modificar la tienda en línea propia de un negocio que vende con Ami, a través de la [API de tiendas](https://docs.amiagente.com): catálogo, carrito, cotización, pedidos con pago en la página de Ami, citas, reservas, suscripciones y webhooks. |

## Instalar

En la carpeta de tu proyecto, con la CLI de [skills](https://skills.sh):

```bash
npx skills add agventures/ami-skills
```

Te pregunta para qué agentes lo instalas y lo pone en la carpeta que lee cada
uno. `npx skills update` lo trae al día cuando cambia.

En Claude Code también puedes instalarlo como plugin:

```text
/plugin marketplace add agventures/ami-skills
/plugin install ami-storefront@ami-skills
```

Sin la CLI, copia la carpeta `skills/ami-storefront` a `.agents/skills/` de tu
proyecto (Codex, Cursor y la mayoría) o a `.claude/skills/` (Claude Code).

## Para empezar

- Una llave de prueba (`ami_test_…`): la crea el dueño del negocio en
  **Ajustes › Desarrolladores** y va en `AMI_API_KEY`, en el servidor. Con
  ella el agente ve los productos reales del negocio y prueba la compra
  completa sin vender nada.
- [Construir con agentes](https://docs.amiagente.com/docs/agentes): qué
  pedirle al agente y cómo revisar lo que entrega.
- [La tienda de ejemplo](https://github.com/agventures/ami-storefront-demo):
  una tienda completa en Next.js que ya trae este skill.

Este repositorio se publica desde el código de Ami, así que no se edita aquí.

## Licencia

MIT. Ver [LICENSE](./LICENSE).
