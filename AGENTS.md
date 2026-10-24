# Writing recipes for this site

This is a family recipe book. Recipes are cooked by a parent together with young children: the children follow the ingredient pictures, the adult reads the method. Write so both can use it.

## Voice and style

- Write the way a parent in a British (Scottish) family living in Sweden would talk in the kitchen: friendly, plain, a bit playful.
- British spelling and words: colour, yoghurt, icing sugar, bicarb, baking tray, clingfilm, tin, hob.
- Light, informal words are welcome where they fit: "squish", "splodges", "shoogle", "dollop", "blobs".
- An occasional short aside or warning with an exclamation mark is fine: "(it will be really sticky!)", "Watch carefully so they do not burn!", "Eat excess mixtures!". Use one or two per recipe at most.
- Use real kitchen equipment the family has where it matters: "a square glass Ikea box", "a stick blender", "a waffle iron".
- Swedish bakes keep their Swedish names (kanelbullar, lussebullar, kladdkaka, pepparkakor, bullar).
- Assume the adult knows basic techniques (rub in, cream, fold, knead, prove). Don't explain them.
- Keep it short. No introduction, story, nutrition info or serving suggestions beyond a few words.

## File and front matter

- One Markdown file per recipe in `_sweet/` or `_savory/`. File name is lowercase with underscores, e.g. `_sweet/lemon_scones.md`.
- Front matter, exactly these keys:

```yaml
---
layout: recipes
name: Lemon Scones
title: "Lemon Scones"
image: /img/lemonscones.jpg
---
```

- `name` and `title` are the same, in Title Case. `image` is a photo of the finished bake in `/img/`.

## Page structure

In this order, with a blank line between each part:

1. Oven line, if the oven is used: `Preheat oven to 180°C`. Use °C with no space. If the oven is only heated after a long rise, put it as a method step instead ("Heat oven to 230°C.").
2. `Ingredients:` followed by the picture table.
3. `Method:` followed by numbered steps.
4. If the recipe came from somewhere else: `Original recipe from: <url>`.

If the recipe has separate parts (dough and filling, cake and icing), give each part its own labelled table, e.g. `Ingredients for cupcakes:` and `Ingredients for icing:`. Put a separate `Method:` after each part if the parts are made at different times.

## Ingredient table

- Three ingredients per row. Each row of ingredients is two table lines: pictures, then amounts.

```
| ![Flour](/img/flour.jpg){:height="100px"} | ![Butter](/img/butter.jpg){:height="100px"} | ![Sugar](/img/sugar.jpg){:height="100px"} |
| 250 g plain flour | 50 g butter | 30 g sugar |
```

- Every picture is `{:height="100px"}`. Alt text is the ingredient name in sentence case.
- Reuse the existing images in `/img/` (e.g. `flour.jpg`, `egg.jpg`, `salt.jpg`). Check the folder before inventing a new file name. If a new image is needed, name it lowercase with no spaces (`pearlsugar.jpg`) and tell the user it needs adding.
- Fill empty cells in the last row with `|  |`.
- List ingredients in the order they are used in the method.
- Amounts: number, space, unit, ingredient — `250 g plain flour`, `1 teaspoon salt`, `1.5 dl oats`, `2 eggs`.
  - Grams for most dry ingredients and butter; `dl` for oats and cup-style measures; `ml` for liquids.
  - Write `teaspoon(s)` and `tablespoon(s)` in full, never tsp/tbsp.
  - Use decimals (0.5) rather than fractions where possible.

## Method

- Numbered list, one main action per step, short imperative sentences starting with a verb: "Mix…", "Add…", "Roll out to 2 cm thick.", "Bake for 12 minutes."
- Name every ingredient in the step that uses it, so it can be matched to its picture and none are missed. Don't write "all flours" or "the dry ingredients" — write "plain flour, rye flour and wholemeal flour".
- "Mix all ingredients together" (or "all the sauce ingredients", "everything") is fine when every ingredient in the recipe, or in that part of it, goes in at once. No list is needed.
- When there are exceptions — "all other ingredients", "everything except…", "the rest of the ingredients" — follow the phrase with the ingredients in brackets so none are missed: "Mix with all other brownie ingredients (egg, sugar, flour, baking powder, cocoa powder and vanilla)."
- Give times, sizes and quantities in the step: "leave to rise for 30 minutes", "split into 8 rolls", "about 0.5 cm thick", "a 20 cm cake tin".
- Use simple cues for when something is ready: "until it bubbles", "until light and fluffy", "until it is not sticky anymore".
- End each step with a full stop. The last step is usually the bake time.
