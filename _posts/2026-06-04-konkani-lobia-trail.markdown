---
layout: post
title: "Dehydrated Konkani Lobia for the Trail"
date: 2026-06-04
categories: [Backpacking]
---

A tangy black-eyed pea curry, dehydrated and trail-ready. This one has been tested on multi-day trips and holds up well — rehydrates nicely and actually tastes like real food after a long day.

![Konkani Lobia on the trail](/assets/images/lobia.jpg){: style="width:100%; border-radius:12px; margin: 1em 0;"}

---

**Flavor profile:** Mildly tangy with a good coconut base. Cumin and coriander should come through clearly — worth making your own powders at home before the trip.

For cumin: dry roast on a cast iron, medium heat, stirring constantly for ~30 seconds until you get that earthy smell. If it burns even slightly, toss and start over — it turns bitter fast.

For coriander: same pan, medium heat, ~40 seconds until fragrant.

**Heat:** Mild to medium. Solid for a cold night out.

**Note:** Dehydration takes some of the spice away. Option — carry a small bag of extra cumin+coriander powder and dehydrated green chili powder (chop green chilies, dehydrate, pulse in a blender) to adjust on trail.

---

## Serving Size

<div style="margin: 1em 0;">
  <label for="servings" style="font-weight: bold;">Servings: </label>
  <button onclick="updateServings2(-1)" style="padding: 2px 10px; font-size: 1em;">−</button>
  <span id="servings-display2" style="margin: 0 10px; font-size: 1.1em; font-weight: bold;">4</span>
  <button onclick="updateServings2(1)" style="padding: 2px 10px; font-size: 1em;">+</button>
</div>

<script>
  const BASE2 = 4;
  let current2 = 4;

  const ingredients2 = {
    rice: { base: 2, unit: "cups", label: "dehydrated rice" },
    curry: { base: 1.25, unit: "cups", label: "dehydrated curry (see below)" },
    coconut_milk: { base: 4, unit: "tbsp", label: "coconut milk powder" },
    tamarind: { base: 2, unit: "pieces", label: "tamarind" },
    mustard: { base: 0.5, unit: "tsp", label: "black mustard seeds" },
    curry_leaves: { base: 8, unit: "", label: "curry leaves" },
    cumin: { base: 0.5, unit: "tsp", label: "cumin powder (home roasted)" },
    coriander: { base: 0.5, unit: "tsp", label: "coriander powder (home roasted)" },
    garlic_onion: { base: 1, unit: "tbsp", label: "dehydrated garlic+onion granules" },
    red_chili: { base: 1, unit: "tsp", label: "red chili powder" },
    oil: { base: 1, unit: "tbsp", label: "oil" },
    asafoetida: { base: 0.25, unit: "tsp", label: "asafoetida (hing)" },
    squash: { base: 0.5, unit: "cup", label: "dehydrated butternut squash (optional)" },
  };

  function fmt2(val) {
    const fractions = [[0.125,"⅛"],[0.25,"¼"],[0.33,"⅓"],[0.5,"½"],[0.67,"⅔"],[0.75,"¾"]];
    const whole = Math.floor(val);
    const dec = parseFloat((val - whole).toFixed(2));
    const frac = fractions.find(f => Math.abs(f[0] - dec) < 0.04);
    if (whole === 0) return frac ? frac[1] : val.toFixed(1);
    if (!frac || dec === 0) return whole % 1 === 0 ? whole : val.toFixed(1);
    return whole + frac[1];
  }

  function updateServings2(delta) {
    current2 = Math.max(1, current2 + delta);
    document.getElementById("servings-display2").textContent = current2;
    const ratio = current2 / BASE2;
    for (const [key, ing] of Object.entries(ingredients2)) {
      const el = document.getElementById("ing2-" + key);
      if (el) el.textContent = fmt2(ing.base * ratio) + (ing.unit ? " " + ing.unit : "");
    }
  }
</script>

---

## Ingredients

**Trail pack**
- <span id="ing2-rice">2 cups</span> dehydrated rice
- <span id="ing2-curry">1¼ cups</span> dehydrated curry (see below)
- <span id="ing2-coconut_milk">4 tbsp</span> coconut milk powder
- <span id="ing2-tamarind">2 pieces</span> tamarind
- <span id="ing2-mustard">½ tsp</span> black mustard seeds
- <span id="ing2-curry_leaves">8</span> curry leaves
- <span id="ing2-cumin">½ tsp</span> cumin powder (home roasted)
- <span id="ing2-coriander">½ tsp</span> coriander powder (home roasted)
- <span id="ing2-garlic_onion">1 tbsp</span> dehydrated garlic+onion granules
- <span id="ing2-red_chili">1 tsp</span> red chili powder
- <span id="ing2-oil">1 tbsp</span> oil
- <span id="ing2-asafoetida">¼ tsp</span> asafoetida (hing)
- <span id="ing2-squash">½ cup</span> dehydrated butternut squash (optional)

---

## At Home — Dehydrating the Curry

**1. Cook the curry (Instant Pot)**
Sauté mustard seeds in oil until they crackle. Add curry leaves, cumin, coriander, garlic, onion, and tomatoes. Cook until tomatoes soften, about 3 minutes. Add cayenne, black-eyed peas, salt, and 2 cups water. Pressure cook on high for 10 minutes. Let simmer to reduce excess water after cooking.

**2. Dehydrate the curry**
Spread cooked curry thinly on dehydrator trays. Dehydrate at 135°F for 8–10 hours until completely dry and crumbly. Break into pieces and store in a zip-lock bag.

**3. Dehydrate the butternut squash (optional)**
Steam in Instant Pot for 1 minute. Spread on dehydrator trays at 135°F for 8 hours.

**4. Dehydrate the rice**
Cook rice normally. Spread on dehydrator trays at 135°F for 6–8 hours until dry and separate.

---

## On the Trail

**1. Rehydrate**
Soak tamarind in a little hot water. Optionally rehydrate beans and squash separately to reduce cook time.

**2. Cook**
Heat oil in your pot. Add mustard seeds — once they splutter, add garlic/onion granules, red chili, and curry leaves. Add dehydrated curry, tamarind water, and enough water to cover. Dissolve coconut milk powder in water and add. Adjust water as needed.

**3. Simmer**
Cook for ~15 minutes, stirring occasionally, until everything is rehydrated and the curry is thick.

**4. Rice**
Rehydrate rice with water at a 1:1.2 ratio (rice:water).

**5. Serve**
Ladle curry over rice. Adjust spice with extra cumin/coriander powder or green chili powder if needed.

---

## Notes

**Spice adjustment on trail:** Dehydration mellows the spices. Carry a small bag of extra cumin+coriander powder and dehydrated green chili powder — chop green chilies, dehydrate, then pulse in a blender. Adds heat and freshness.

**Scaling up:** For ~20 servings, use 2 cups dry black-eyed peas with 2 cups water in the IP. High pressure, 10 minutes, then simmer to reduce.

**Butternut squash:** Steam 1 minute in IP, dehydrate at 135°F for 8 hours.

---

*Adapted from Rinku Bhattacharya's Konkani Lobia in* Instant Indian *(Hippocrene Books), via Epicurious. Trail-adapted and dehydrated for backpacking.*