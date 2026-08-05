# 4. Create the Item Details Screen

The **Item Details** screen gives the user a closer look at the Iced Latte before adding it to an order.

In this section, you will reuse elements from the Menu screen and reformat them for a detailed product view.

## 4.1. Duplicate and Clear the Menu Screen

1. Select `01 Menu`.
2. Duplicate it:

   - Windows: `Ctrl + D`
   - Mac: `Command + D`

3. Move the duplicate to the right of `01 Menu`.
4. Rename it:

   ```text
   02 Item Details
   ```

5. Expand `02 Item Details` in the Layers panel.
6. Delete all existing content inside it, but do not delete the phone frame itself.

The duplicated screen should retain:

- The Android Compact dimensions
- `Colour / Background`
- Horizontal padding of `24`
- Vertical padding of `48`
- Vertical auto layout

## 4.2. Create the Back Button

Reuse an existing `View Item` button.

1. Expand one of the menu-item cards inside `01 Menu`.
2. Select its `Button / View Item` frame.
3. Copy the button:

   - Windows: `Ctrl + C`
   - Mac: `Command + C`

4. Select `02 Item Details`.
5. Paste the button:

   - Windows: `Ctrl + V`
   - Mac: `Command + V`

6. Confirm that the button is nested inside `02 Item Details`.
7. Rename it:

   ```text
   Button / Back
   ```

8. Change the text inside the button to:

   ```text
   < Back
   ```

9. Change the button-text size to `14`.
10. Keep the button frame set to:

   - Width: **Hug contents**
   - Height: **Hug contents**
   - Horizontal padding: `16`
   - Vertical padding: `8`
   - Fill: `Colour / Primary`
   - Corner radius: `8`
   - Content alignment: **Centre**

## 4.3. Add the Large Product Image

Reuse the Iced Latte image background from the Menu screen.

1. In `01 Menu`, expand `Card / Iced Latte`.
2. Select `Image Background`.
3. Copy and paste it into `02 Item Details`.
4. Confirm that `Image Background` is nested directly inside `02 Item Details`.
5. Configure it using:

   - Width: **Fill container**
   - Height: `200`
   - Padding: `8`
   - Fill: `Colour / Placeholder`
   - Corner radius: `12`

6. Select the `Image` rectangle inside it.
7. Confirm that the image remains:

   - Width: **Fill container**
   - Height: **Fill container**
   - Fill style: `Image/Iced Latte`
   - Image scaling: **Fit**

The image should expand with the larger frame while remaining fully visible.

## 4.4. Add and Reformat the Item Information

Reuse the Iced Latte information from the Menu screen.

1. In `01 Menu`, expand `Card / Iced Latte`, then expand `Card Right`.
2. Select `Information`.
3. Copy and paste it into `02 Item Details`.
4. Confirm that `Information` is nested directly inside `02 Item Details`.

### Configure the Information Frame

Select `Information` and set:

- Direction: **Vertical**
- Gap: `16`
- Alignment: **Top left**
- Width: **Fill container**
- Height: **Hug contents**

### Configure Name + Description

Select `Name + Description` and set:

- Direction: **Vertical**
- Gap: `4`
- Alignment: **Top left**
- Width: **Fill container**
- Height: **Hug contents**

### Reformat the Text Layers

Select each text layer and apply:

#### Name

- Text: `Iced Latte`
- Weight: Bold
- Size: `28`
- Text alignment: Left

#### Description

- Text: `Espresso, milk and ice`
- Weight: Regular
- Size: `14`
- Text alignment: Left

#### Price

- Text: `$4.50`
- Weight: Semi Bold
- Size: `20`
- Text alignment: Left

Keep all three text layers filled with `Colour / Text`.

## 4.5. Group the Main Content

1. Select:

   - `Button / Back`
   - `Image Background`
   - `Information`

2. Press `Shift + A`.
3. Rename the new frame:

   ```text
   Details Content
   ```

4. Configure it using:

   - Direction: **Vertical**
   - Gap: `24`
   - Alignment: **Top left**
   - Width: **Fill container**
   - Height: **Hug contents**

The hierarchy should be:

```text
Details Content
├── Button / Back
├── Image Background
│   └── Image
└── Information
    ├── Name + Description
    │   ├── Name
    │   └── Description
    └── Price
```

## 4.6. Create the Add to Order Button

1. Select `Button / Back`.
2. Duplicate it.
3. Move the duplicate outside `Details Content` so it is nested directly inside `02 Item Details`, underneath `Details Content`.
4. Rename it:

   ```text
   Button / Add to Order
   ```

5. Change the text to:

   ```text
   Add to Order
   ```

6. Configure the button frame using:

   - Width: **Fill container**
   - Height: **Hug contents**
   - Padding: `16` on all sides
   - Fill: `Colour / Primary`
   - Corner radius: `8`
   - Content alignment: **Centre**

7. Configure the text using:

   - Font: Inter
   - Weight: Semi Bold
   - Size: `16`
   - Fill: `Colour / Surface`
   - Text alignment: Centre

## 4.7. Position the Bottom Button

1. Select `02 Item Details`.
2. Change the screen gap to **Auto**.
3. Keep:

   - Direction: **Vertical**
   - Alignment: **Top left**
   - Horizontal padding: `24`
   - Vertical padding: `48`

The automatic gap places `Details Content` near the top and `Button / Add to Order` near the bottom.

The completed structure should be:

```text
02 Item Details
├── Details Content
│   ├── Button / Back
│   ├── Image Background
│   │   └── Image
│   └── Information
│       ├── Name + Description
│       │   ├── Name
│       │   └── Description
│       └── Price
└── Button / Add to Order
```

## 4.8. Item Details Screen Checkpoint

Your Item Details screen should contain:

- [ ] A frame named `02 Item Details`
- [ ] A `Button / Back` displaying `< Back`
- [ ] A `200` px-high image background
- [ ] An image that fills the background and uses `Image/Iced Latte`
- [ ] Left-aligned item information
- [ ] A `Name + Description` gap of `4`
- [ ] An `Information` gap of `16`
- [ ] A `Details Content` gap of `24`
- [ ] A full-width `Button / Add to Order`
- [ ] An automatic gap between the main content and bottom button

Do not add prototype connections yet.

---

[Next: Section 5 – Create the Order Summary Screen](05-create-the-order-summary-screen.md)
