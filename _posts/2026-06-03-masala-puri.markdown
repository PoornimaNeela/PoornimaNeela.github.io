---
layout: post
title: "Bangalore Style Masala Puri"
date: 2026-06-03
categories: chaat street-food bangalore
---

If there's one dish that makes me instantly homesick for Bangalore, it's masala puri. Not the chickpea versions you find outside Karnataka – the real deal: a thick, greenish pea masala ladled over crushed puris, topped with sev, raw onion, carrot, and a squeeze of lime. :)

The spice blend is the heart of it – don't skip the marathi moggu if you can find it at an Indian grocery store.

![Bangalore-style masala puri](/assets/images/Masala_puri.jpg){: style="width:100%; border-radius:12px; margin: 1em 0;"}
---

## Serving Size

<div style="margin: 1em 0;">
  <label for="servings" style="font-weight: bold;">Servings: </label>
  <button onclick="updateServings(-1)" style="padding: 2px 10px; font-size: 1em;">−</button>
  <span id="servings-display" style="margin: 0 10px; font-size: 1.1em; font-weight: bold;">4</span>
  <button onclick="updateServings(1)" style="padding: 2px 10px; font-size: 1em;">+</button>
</div>

<script>
  const BASE = 4;
  let current = 4;

  const ingredients = {
    vatana: { base: 2, unit: "cups", label: "dried green vatana, soaked overnight" },
    potato: { base: 1, unit: "", label: "small potato" },
    carrot_ip: { base: 1, unit: "", label: "carrot (cooked with vatana in IP)" },
    water: { base: 3, unit: "cups", label: "water (for IP)" },
    coriander_seeds: { base: 1.5, unit: "tsp", label: "coriander seeds" },
    cumin_seeds: { base: 0.5, unit: "tsp", label: "cumin seeds" },
    peppercorns: { base: 0.75, unit: "tsp", label: "black peppercorns" },
    fennel_seeds: { base: 0.5, unit: "tsp", label: "fennel seeds" },
    cloves: { base: 3, unit: "", label: "cloves" },
    cinnamon: { base: 1, unit: "inch", label: "cinnamon stick" },
    moggu: { base: 2, unit: "", label: "marathi moggu (kapok buds)" },
    chana_dal: { base: 1.5, unit: "tsp", label: "roasted chana dal" },
    mace: { base: 1, unit: "strand", label: "mace" },
    green_chili: { base: 2, unit: "", label: "green chilies" },
    garlic: { base: 2, unit: "cloves", label: "garlic" },
    ginger: { base: 0.5, unit: "tbsp", label: "ginger, roughly chopped" },
    coconut: { base: 1, unit: "tbsp", label: "fresh coconut, grated" },
    tomato_paste: { base: 0.5, unit: "", label: "roma tomato (for paste)" },
    tamarind: { base: 1, unit: "tbsp", label: "tamarind paste" },
    jaggery: { base: 1.5, unit: "tsp", label: "jaggery" },
    sugar: { base: 0.5, unit: "tsp", label: "sugar" },
    chaat_masala: { base: 1.5, unit: "tsp", label: "chaat masala" },
    fennel_powder: { base: 0.25, unit: "tsp", label: "fennel powder" },
    kala_namak: { base: 1, unit: "tsp", label: "kala namak" },
    salt: { base: 0.75, unit: "tsp", label: "salt, to taste" },
    oil: { base: 2, unit: "tbsp", label: "oil" },
    curry_leaves: { base: 10, unit: "", label: "curry leaves" },
    puris: { base: 40, unit: "", label: "small crispy puris (pani puri shells)" },
    onion: { base: 1, unit: "", label: "onion, very finely diced" },
    tomato_top: { base: 1, unit: "", label: "tomato, finely diced" },
    carrot_top: { base: 1, unit: "", label: "carrot, grated (for topping)" },
    coriander_top: { base: 0.33, unit: "cups", label: "coriander leaves, chopped (for topping)" },
    sev: { base: 0.75, unit: "cups", label: "fine sev" },
    chutney: { base: 4, unit: "tbsp", label: "sweet tamarind-date chutney" },
    lime: { base: 1, unit: "", label: "lime, cut into wedges" },
  };

  function fmt(val) {
    const fractions = [[0.125,"⅛"],[0.25,"¼"],[0.33,"⅓"],[0.5,"½"],[0.67,"⅔"],[0.75,"¾"]];
    const whole = Math.floor(val);
    const dec = parseFloat((val - whole).toFixed(2));
    const frac = fractions.find(f => Math.abs(f[0] - dec) < 0.04);
    if (whole === 0) return frac ? frac[1] : val.toFixed(1);
    if (!frac || dec === 0) return whole % 1 === 0 ? whole : val.toFixed(1);
    return whole + frac[1];
  }

  function updateServings(delta) {
    current = Math.max(1, current + delta);
    document.getElementById("servings-display").textContent = current;
    const ratio = current / BASE;
    for (const [key, ing] of Object.entries(ingredients)) {
      const el = document.getElementById("ing-" + key);
      if (el) el.textContent = fmt(ing.base * ratio) + (ing.unit ? " " + ing.unit : "");
    }
  }
</script>

---

## Ingredients

**Cook the peas**
- <span id="ing-vatana">2 cups</span> dried green vatana, soaked overnight
- <span id="ing-potato">1</span> small potato
- <span id="ing-carrot_ip">1</span> carrot (cooked with vatana in IP)
- <span id="ing-water">3 cups</span> water (for IP)
- Pinch of salt

**Whole spices (dry roast)**
- <span id="ing-coriander_seeds">1½ tsp</span> coriander seeds
- <span id="ing-cumin_seeds">½ tsp</span> cumin seeds
- <span id="ing-peppercorns">¾ tsp</span> black peppercorns
- <span id="ing-fennel_seeds">½ tsp</span> fennel seeds
- <span id="ing-cloves">3</span> cloves
- <span id="ing-cinnamon">1 inch</span> cinnamon stick
- <span id="ing-moggu">2</span> marathi moggu (kapok buds)
- <span id="ing-chana_dal">1½ tsp</span> roasted chana dal

**Masala paste**
- <span id="ing-mace">1 strand</span> mace
- Pinch of nutmeg
- <span id="ing-green_chili">2</span> green chilies
- <span id="ing-garlic">2 cloves</span> garlic
- <span id="ing-ginger">½ tbsp</span> ginger, roughly chopped
- <span id="ing-coconut">1 tbsp</span> fresh coconut, grated
- <span id="ing-tomato_paste">½</span> roma tomato
- Handful of coriander leaves
- Handful of mint leaves
- <span id="ing-tamarind">1 tbsp</span> tamarind paste

**Gravy seasoning**
- <span id="ing-jaggery">1½ tsp</span> jaggery
- <span id="ing-sugar">½ tsp</span> sugar
- <span id="ing-chaat_masala">1½ tsp</span> chaat masala
- <span id="ing-fennel_powder">¼ tsp</span> fennel powder
- <span id="ing-kala_namak">1 tsp</span> kala namak
- <span id="ing-salt">¾ tsp</span> salt, to taste
- <span id="ing-oil">2 tbsp</span> oil
- <span id="ing-curry_leaves">10</span> curry leaves

**Assembly**
- <span id="ing-puris">40</span> small crispy puris (pani puri shells)
- <span id="ing-onion">1</span> onion, very finely diced
- <span id="ing-tomato_top">1</span> tomato, finely diced
- <span id="ing-carrot_top">1</span> carrot, grated
- <span id="ing-coriander_top">⅓ cup</span> coriander leaves, chopped
- <span id="ing-sev">¾ cup</span> fine sev
- <span id="ing-chutney">4 tbsp</span> sweet tamarind-date chutney
- <span id="ing-lime">1</span> lime, cut into wedges

---

## Steps

**1. Cook the vatana**
Add soaked vatana, whole potato, carrot, water, and a pinch of salt to the Instant Pot. High pressure, 14 minutes, natural release 10 minutes then quick release. Remove the potato and carrot and set aside. Reserve all cooking liquid — it's starchy and seasoned, you'll need it.

**2. Dry roast the whole spices**
In a dry skillet over medium heat, roast coriander seeds, cumin seeds, peppercorns, fennel seeds, cloves, cinnamon, and marathi moggu together until fragrant and lightly darkened, about 2 minutes. Remove. In the same pan, roast the chana dal separately until golden — it browns faster. Cool everything before blending.

**3. Make the masala paste**
Blend roasted spices and chana dal with mace, nutmeg, green chilies, garlic, ginger, coconut, tomato, coriander leaves, mint leaves, and tamarind paste into a very smooth paste with a little water. Blend thoroughly — texture matters here.

**4. Cook the masala paste**
Heat oil in a deep pan. Add curry leaves and let them splutter. Add the masala paste and cook on medium, stirring frequently, until the oil separates and the paste darkens — 8 to 10 minutes. Don't rush this step.

**5. Build and simmer the gravy**
Add about 1 cup reserved cooking liquid. Stir in jaggery, sugar, chaat masala, fennel powder, kala namak, and salt. Mash about ¼ of the cooked vatana into the gravy to thicken. Add remaining peas whole. Simmer 20–25 minutes on low, adjusting consistency with more cooking liquid. Should be thick but pourable.

**6. Prep for assembly**
Soak diced onion in ice cold water for 10–15 minutes — this removes the bite. Drain well before serving.

**7. Assemble and serve**
Crush 8–10 puris into each bowl. Ladle hot pea masala generously over. Top with diced tomato, grated carrot, drained onion, a drizzle of tamarind-date chutney, fresh coriander, and a big handful of sev. Squeeze lime over everything and eat immediately — this does not wait.

---

## Notes

**Cooking liquid:** Don't discard — it's the secret to a good gravy.

**Rest time:** The gravy tastes best after a few hours or the next day. Reheat well before serving.

**Marathi moggu:** Find these at Karnataka or South Indian grocery stores. If unavailable, sub with an extra clove and a tiny pinch of allspice.

**Green vs orange masala:** This recipe gives a greenish masala. For a more orange version, reduce coriander leaves to 2 stalks and add 1 extra tsp coriander seeds instead.