[Previous: Section 1 – Getting Started](01-getting-started-in-figma.md)

# 2. Design Reference

Use the colours and sample menu information below while creating your café app. Using the same reference information will make it easier to follow the tutorial and compare your work with the demonstrated example.

You may customize the app later if you finish early.

## 2.1. Colour Palette

Before designing the café app, you will create reusable colour styles and a visual colour palette on the canvas.

Saving the colours as styles will keep your design consistent and prevent you from repeatedly entering the same hex codes. The visible colour swatches will also give you a quick reference while you work.

### Create the Six-Swatch Palette

1. Press `R` to select the **Rectangle** tool.
2. Draw a `24 × 24` pixel square anywhere outside your phone frames.
3. Add a `2` px black stroke and set the stroke alignment to **Inside**.
4. With the rectangle selected, press `Shift + A` to place it inside an auto-layout frame.
5. Configure the auto-layout frame using the following settings:

   - Direction: **Horizontal**
   - Gap between items: `4`
   - Alignment: **Centre**
   - Padding: `4` on all sides
   - Width: **Hug contents**
   - Height: **Hug contents**
   - Fill: White

6. Rename the auto-layout frame:

   ```text
   Colour Palette
   ```

7. Select the rectangle inside `Colour Palette`.
8. Duplicate the rectangle five times so the frame contains six swatches:

   - Windows: `Ctrl + D`
   - Mac: `Command + D`

Because the rectangle is already inside an auto-layout frame, each duplicate will appear beside the previous swatch instead of overlapping it.

9. Confirm that six swatches are visible inside the frame.

### Assign and Save Each Colour

Work through the six swatches from left to right.

For each swatch:

1. Select the swatch.
2. Open the **Fill** colour picker in the right sidebar.
3. Enter the corresponding hex code from the table below.
4. Open the style controls beside **Fill**.
5. Select **Create style** or the `+` button.
6. Enter the corresponding style name from the table.
7. Select **Create style**.
8. Rename the swatch layer using the corresponding layer name.

| Style Name | Hex Code | Suggested Layer Name | Use |
|---|---:|---|---|
| `Colour / Primary` | `#5A3825` | `Swatch / Primary` | Buttons and primary actions |
| `Colour / Background` | `#F7F3EE` | `Swatch / Background` | Phone-screen backgrounds |
| `Colour / Placeholder` | `#E8D8C5` | `Swatch / Placeholder` | Product-image backgrounds |
| `Colour / Surface` | `#FFFFFF` | `Swatch / Surface` | Cards and light foreground elements |
| `Colour / Text` | `#241A14` | `Swatch / Text` | Main interface text |
| `Colour / Success` | `#357A38` | `Swatch / Success` | Confirmation and success elements |

### Apply a Saved Colour Style

When a later step tells you to apply a colour style:

1. Select the object.
2. Find **Fill** in the right sidebar.
3. Open the style picker.
4. Select the requested style.

For example, choosing `Colour / Primary` applies the saved brown colour without requiring the hex code again.

## 2.2. Sample Menu Items

Use the following information throughout the tutorial:

| Item | Description | Price | Image |
|---|---|---:|---|
| Iced Latte | Espresso, milk and ice | `$4.50` | Supplied Iced Latte image |
| Blueberry Muffin | Baked fresh this morning | `$3.25` | Supplied Blueberry Muffin image |
| Grilled Cheese | Cheddar on toasted sourdough | `$6.50` | Supplied Grilled Cheese image |

The main prototype path will use the Iced Latte:

`Menu` → `Iced Latte Details` → `Order Summary` → `Confirmation`

Only the Iced Latte requires a detailed item screen in this tutorial. The other menu items will appear on the Menu screen but will not be connected in the prototype.

---

[Next: Section 3 – Create the Menu Screen](03-create-the-menu-screen.md)
