## Tutorial Sections

1. [Getting Started in Figma](01-getting-started-in-figma.md)
2. [Design Reference](02-design-reference.md)
3. **Create the Menu Screen**
4. [Create the Item Details Screen](04-create-the-item-details-screen.md)
5. [Create the Order Summary Screen](05-create-the-order-summary-screen.md)
6. [Create the Confirmation Screen](06-create-the-confirmation-screen.md)
7. [Connect and Test the Prototype](07-connect-and-test-the-prototype.md)

---

# 3. Create the Menu Screen

The **Menu** screen is the first screen users will see when they open the café app. It introduces the café and displays three available menu items.

In this section, you will:

- Create your first phone screen.
- Organize the screen using auto layout.
- Add headings and supporting text.
- Create a reusable menu-item card.
- Add and save product-image styles.
- Duplicate and edit repeated interface elements.

## 3.1. Create an Android Compact Frame

1. Press `F` to select the **Frame** tool.
2. In the right sidebar, find the Android device presets.
3. Select **Android Compact**.

The preset creates a `412 × 917` frame automatically.

4. Rename the frame:

   ```text
   01 Menu
   ```

5. Apply the following settings to `01 Menu`:

   - Direction: **Vertical**
   - Gap between items: `24`
   - Alignment: **Top left**
   - Horizontal padding: `24`
   - Vertical padding: `48`
   - Fill: `Colour / Background`

## 3.2. Add the Page Header

Create the café name and subtitle as separate text layers before grouping them.

### Create the Café Name

1. Press `T`.
2. Click inside `01 Menu`.
3. Enter:

   ```text
   Campus Café
   ```

4. Rename the text layer:

   ```text
   Title
   ```

5. Apply:

   - Font: Inter
   - Weight: Bold
   - Size: `28`
   - Fill: `Colour / Text`
   - Text alignment: Left

### Create the Subtitle

1. Press `T`.
2. Create another text layer underneath the title.
3. Enter:

   ```text
   Order ahead and skip the line.
   ```

4. Rename the text layer:

   ```text
   Subtitle
   ```

5. Apply:

   - Font: Inter
   - Weight: Regular
   - Size: `14`
   - Fill: `Colour / Text`
   - Text alignment: Left

### Group the Title and Subtitle

1. Select `Title` and `Subtitle`.
2. Press `Shift + A`.
3. Rename the new frame:

   ```text
   Title + Subtitle
   ```

4. Configure it using:

   - Direction: **Vertical**
   - Gap: `8`
   - Alignment: **Top left**
   - Width: **Fill container**
   - Height: **Hug contents**

The `01 Menu` frame's `24` px gap will control the spacing between this header and the next screen element.

## 3.3. Add the Section Heading

1. Press `T`.
2. Create a text layer inside `01 Menu`, underneath `Title + Subtitle`.
3. Enter:

   ```text
   Popular Today
   ```

4. Rename the layer:

   ```text
   Popular Today
   ```

5. Apply:

   - Font: Inter
   - Weight: Semi Bold
   - Size: `18`
   - Fill: `Colour / Text`
   - Text alignment: Left

Do not add manual spacing. The screen's auto-layout gap places this heading `24` px below the header.

## 3.4. Create the Iced Latte Card

### Create the Card Frame

1. Press `F`.
2. Draw a frame underneath `Popular Today`.
3. Press `Shift + A` to apply auto layout.
4. Rename the frame:

   ```text
   Card / Iced Latte
   ```

5. Configure the card using:

   - Direction: **Horizontal**
   - Width: **Fill container**
   - Height: `140`
   - Gap: **Auto**
   - Padding: `12` on all sides
   - Alignment: **Centre**
   - Fill: `Colour / Surface`
   - Corner radius: `16`

### Create the Image Background

1. Press `F`.
2. Draw a frame inside `Card / Iced Latte`.
3. Rename it:

   ```text
   Image Background
   ```

4. Configure it using:

   - Aspect ratio: **Square**
   - Height: **Fill container**
   - Fill: `Colour / Placeholder`
   - Corner radius: `12`
   - Padding: `8` on all sides

The square aspect ratio determines the width automatically from the available height.

### Add the Product Image

1. Press `R`.
2. Draw a rectangle inside `Image Background`.
3. Rename it:

   ```text
   Image
   ```

4. Set:

   - Width: **Fill container**
   - Height: **Fill container**

5. Open the rectangle's **Fill** settings.
6. Choose **Image** and select the supplied Iced Latte image.
7. Set the image scaling to **Fit**.
8. Save the image fill as a style named:

   ```text
   Image/Iced Latte
   ```

The entire image should remain visible without being cropped.

## 3.5. Create the Card Information

### Create the Card Right Frame

1. Press `F`.
2. Draw a frame inside `Card / Iced Latte`, beside `Image Background`.
3. Press `Shift + A`.
4. Rename it:

   ```text
   Card Right
   ```

5. Configure it using:

   - Direction: **Vertical**
   - Gap: **Auto**
   - Alignment: **Top right**
   - Width: **Fill container**
   - Height: **Fill container**

### Create the Item Name

1. Press `T`.
2. Click inside `Card Right`.
3. Enter:

   ```text
   Iced Latte
   ```

4. Rename the text layer:

   ```text
   Name
   ```

5. Apply:

   - Font: Inter
   - Weight: Semi Bold
   - Size: `18`
   - Fill: `Colour / Text`
   - Text alignment: Right

### Create the Description

1. Press `T`.
2. Create another text layer inside `Card Right`, underneath `Name`.
3. Enter:

   ```text
   Espresso, milk and ice
   ```

4. Rename it:

   ```text
   Description
   ```

5. Apply:

   - Font: Inter
   - Weight: Regular
   - Size: `12`
   - Fill: `Colour / Text`
   - Text alignment: Right

### Group the Name and Description

1. Select `Name` and `Description`.
2. Press `Shift + A`.
3. Rename the new frame:

   ```text
   Name + Description
   ```

4. Configure it using:

   - Direction: **Vertical**
   - Gap: `4`
   - Alignment: **Top right**
   - Width: **Fill container**
   - Height: **Hug contents**

### Create the Price

1. Press `T`.
2. Create a new text layer inside `Card Right`, underneath `Name + Description`.
3. Enter:

   ```text
   $4.50
   ```

4. Rename it:

   ```text
   Price
   ```

5. Apply:

   - Font: Inter
   - Weight: Semi Bold
   - Size: `16`
   - Fill: `Colour / Text`
   - Text alignment: Right

### Create the Information Frame

1. Select `Name + Description` and `Price`.
2. Press `Shift + A`.
3. Rename the new frame:

   ```text
   Information
   ```

4. Configure it using:

   - Direction: **Vertical**
   - Gap: `8`
   - Alignment: **Top right**
   - Width: **Fill container**
   - Height: **Hug contents**

## 3.6. Create the View Item Button

### Create the Button Label

1. Press `T`.
2. Create a text layer inside `Card Right`, underneath `Information`.
3. Enter:

   ```text
   View Item
   ```

4. Apply:

   - Font: Inter
   - Weight: Semi Bold
   - Size: `12`
   - Fill: `Colour / Surface`
   - Text alignment: Centre

### Apply Auto Layout

1. Select the `View Item` text layer.
2. Press `Shift + A`.
3. Rename the new frame:

   ```text
   Button / View Item
   ```

4. Keep the button inside `Card Right`, directly underneath `Information`.
5. Apply:

   - Fill: `Colour / Primary`
   - Corner radius: `8`
   - Horizontal padding: `16`
   - Vertical padding: `8`
   - Width: **Hug contents**
   - Height: **Hug contents**
   - Content alignment: **Centre**

Because `Card Right` uses an **Auto** gap, `Information` remains at the top and the button remains at the bottom.

## 3.7. Review the First Card

Before duplicating the card, confirm that:

- `Card / Iced Latte` is nested inside `01 Menu`.
- The card uses **Fill container** width and a fixed height of `140`.
- The card has `12` px padding.
- `Image Background` has a square aspect ratio and fills the card height.
- `Image` fills its parent in both directions.
- `Image` uses `Image/Iced Latte` with **Fit** scaling.
- `Card Right` contains `Information` followed by `Button / View Item`.
- Text does not overlap or extend outside the card.

## 3.8. Create the Blueberry Muffin Card

1. Select `Card / Iced Latte`.
2. Duplicate it:

   - Windows: `Ctrl + D`
   - Mac: `Command + D`

Because the card is inside `01 Menu`'s auto layout, the duplicate will appear underneath the first card automatically with a `24` px gap.

3. Rename the duplicate:

   ```text
   Card / Blueberry Muffin
   ```

4. Change the content to:

   - Name: `Blueberry Muffin`
   - Description: `Baked fresh this morning`
   - Price: `$3.25`

5. Select the `Image` rectangle.
6. Replace its image with the supplied Blueberry Muffin image.
7. Keep image scaling set to **Fit**.
8. Save the image fill as:

   ```text
   Image/Blueberry Muffin
   ```

9. Keep the button frame named `Button / View Item`.

This button will remain non-interactive in the final prototype.

## 3.9. Create the Grilled Cheese Card

1. Duplicate `Card / Blueberry Muffin`.
2. Rename the duplicate:

   ```text
   Card / Grilled Cheese
   ```

3. Change the content to:

   - Name: `Grilled Cheese`
   - Description: `Cheddar on toasted sourdough`
   - Price: `$6.50`

4. Replace the product image with the supplied Grilled Cheese image.
5. Keep image scaling set to **Fit**.
6. Save the image fill as:

   ```text
   Image/Grilled Cheese
   ```

7. Keep the button frame named `Button / View Item`.

This button will also remain non-interactive in the final prototype.

## 3.10. Menu Screen Checkpoint

Your Menu screen should contain:

- [ ] A frame named `01 Menu`
- [ ] The Android Compact dimensions
- [ ] `Colour / Background`
- [ ] A `Title + Subtitle` auto-layout frame
- [ ] A `Popular Today` heading
- [ ] Three product cards using **Fill container** width
- [ ] A fixed card height of `140`
- [ ] `24` px between the screen's child elements
- [ ] Three correctly saved image styles
- [ ] Clearly named and nested layers

Do not add prototype connections yet.

---

[Next: Section 4 – Create the Item Details Screen](04-create-the-item-details-screen.md)
