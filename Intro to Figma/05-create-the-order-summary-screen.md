# 5. Create the Order Summary Screen

The **Order Summary** screen allows the user to review the selected item and its total price before placing the order.

In this section, you will reuse the structure of the Item Details screen and copy existing interface elements from the Menu screen.

## 5.1. Duplicate the Item Details Screen

1. Select `02 Item Details`.
2. Duplicate it:

   - Windows: `Ctrl + D`
   - Mac: `Command + D`

3. Move the duplicate to the right of `02 Item Details`.
4. Rename it:

   ```text
   03 Order Summary
   ```

## 5.2. Clear Details Content

1. Expand `03 Order Summary`.
2. Expand `Details Content`.
3. Delete every layer inside `Details Content`.
4. Keep the empty `Details Content` frame.
5. Keep the bottom action button.

Configure `Details Content` using:

- Direction: **Vertical**
- Gap: `24`
- Alignment: **Top left**
- Width: **Fill container**
- Height: **Hug contents**

## 5.3. Update the Bottom Button

1. Select `Button / Add to Order`.
2. Rename it:

   ```text
   Button / Place Order
   ```

3. Change the text inside it to:

   ```text
   Place Order
   ```

Keep:

- Width: **Fill container**
- Height: **Hug contents**
- Padding: `16`
- Fill: `Colour / Primary`
- Corner radius: `8`
- Content alignment: **Centre**
- Text size: `16`
- Text weight: Semi Bold
- Text fill: `Colour / Surface`

## 5.4. Add the Screen Title and Subtitle

1. In `01 Menu`, select `Title + Subtitle`.
2. Copy it.
3. Select `Details Content` inside `03 Order Summary`.
4. Paste the frame.
5. Confirm that it is nested inside `Details Content`.
6. Change the title to:

   ```text
   Your Order
   ```

7. Change the subtitle to:

   ```text
   Review your order before placing it.
   ```

Keep:

- `Title + Subtitle` direction: **Vertical**
- Gap: `8`
- Alignment: **Top left**
- Width: **Fill container**
- Height: **Hug contents**
- Title: `28` px Bold
- Subtitle: `14` px Regular
- Text alignment: Left

## 5.5. Add the Iced Latte Card

1. Select `Card / Iced Latte` inside `01 Menu`.
2. Copy it.
3. Select `Details Content` inside `03 Order Summary`.
4. Paste the card.
5. Confirm that the card appears underneath `Title + Subtitle`.

Keep the card settings:

- Padding: `12`
- Width: **Fill container**
- Height: `140`
- Fill: `Colour / Surface`
- Corner radius: `16`

### Remove the View Item Button

1. Expand `Card / Iced Latte`.
2. Expand `Card Right`.
3. Select `Button / View Item`.
4. Press `Delete` or `Backspace`.

The remaining card structure should be:

```text
Card / Iced Latte
├── Image Background
│   └── Image
└── Card Right
    └── Information
        ├── Name + Description
        │   ├── Name
        │   └── Description
        └── Price
```

Keep `Card Right` set to **Fill container** for both width and height, with its contents aligned to the top right.

## 5.6. Create the Total Row

Create the label and price as separate text layers.

### Create the Total Label

1. Press `T`.
2. Click inside `Details Content`, underneath `Card / Iced Latte`.
3. Enter:

   ```text
   Total
   ```

4. Rename the layer:

   ```text
   Total Label
   ```

5. Apply:

   - Font: Inter
   - Weight: Semi Bold
   - Size: `20`
   - Fill: `Colour / Text`
   - Text alignment: Left

### Create the Total Price

1. Press `T`.
2. Create another text layer beside the label.
3. Enter:

   ```text
   $4.50
   ```

4. Rename the layer:

   ```text
   Total Price
   ```

5. Apply:

   - Font: Inter
   - Weight: Bold
   - Size: `20`
   - Fill: `Colour / Text`
   - Text alignment: Right

### Group the Total Row

1. Select `Total Label` and `Total Price`.
2. Press `Shift + A`.
3. Rename the frame:

   ```text
   Total Row
   ```

4. Configure it using:

   - Direction: **Horizontal**
   - Gap: **Auto**
   - Alignment: **Centre**
   - Width: **Fill container**
   - Height: **Hug contents**

The automatic gap places the label at the left and the price at the right.

## 5.7. Review the Screen Structure

The completed hierarchy should be:

```text
03 Order Summary
├── Details Content
│   ├── Title + Subtitle
│   │   ├── Title
│   │   └── Subtitle
│   ├── Card / Iced Latte
│   │   ├── Image Background
│   │   │   └── Image
│   │   └── Card Right
│   │       └── Information
│   └── Total Row
│       ├── Total Label
│       └── Total Price
└── Button / Place Order
```

Select `03 Order Summary` and confirm:

- Direction: **Vertical**
- Gap: **Auto**
- Alignment: **Top left**
- Horizontal padding: `24`
- Vertical padding: `48`

## 5.8. Order Summary Screen Checkpoint

Your Order Summary screen should contain:

- [ ] A frame named `03 Order Summary`
- [ ] A `Details Content` frame with a `24` px gap
- [ ] A title displaying `Your Order`
- [ ] The subtitle `Review your order before placing it.`
- [ ] An Iced Latte card without a `View Item` button
- [ ] A `Total Row` containing two `20` px text layers
- [ ] A Semi Bold Total label
- [ ] A Bold Total price
- [ ] A full-width `Button / Place Order`
- [ ] An automatic gap between the main content and bottom button

Do not add prototype connections yet.

---

[Next: Section 6 – Create the Confirmation Screen](https://github.com/USERNAME/REPOSITORY/blob/main/06-create-the-confirmation-screen.md)
