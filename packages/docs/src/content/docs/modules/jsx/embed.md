---
title: Embeds
description: How to use Lilybird's Embed components.
sidebar:
  order: 2
---

## Creating embeds

Embeds can easily be created using the main `Embed` component, for properties of the embed you can use the `Embed<x>` versions of said properties.

```tsx
import { Embed, EmbedField, EmbedFooter } from "@lilybird/jsx";

const embed = (
  <Embed title="Hello from Lilybird TSX" color={0xff00ef} timestamp>
    {Array.from({ length: 4 }, (_, i) => (
      <EmbedField name={`Field ${i}`} value="bun" inline />
    ))}
    <EmbedFooter text="Lilybird" />
  </Embed>
);
```
