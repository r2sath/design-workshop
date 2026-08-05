## Tutorial Sections

1. [Getting Started in Figma](01-getting-started-in-figma.md)
2. [Design Reference](02-design-reference.md)
3. [Create the Menu Screen](03-create-the-menu-screen.md)
4. [Create the Item Details Screen](04-create-the-item-details-screen.md)
5. [Create the Order Summary Screen](05-create-the-order-summary-screen.md)
6. **Create the Confirmation Screen**
7. [Connect and Test the Prototype](07-connect-and-test-the-prototype.md)

---

# 6. Create the Confirmation Screen

The **Confirmation** screen tells the user that the order has been placed successfully and provides a way to return to the Menu screen.

## 6.1. Duplicate the Order Summary Screen

1. Select `03 Order Summary`.
2. Duplicate it:

   - Windows: `Ctrl + D`
   - Mac: `Command + D`

3. Move the duplicate to the right of `03 Order Summary`.
4. Rename it:

   ```text
   04 Confirmation
   ```

## 6.2. Clear Details Content

1. Expand `04 Confirmation`.
2. Expand `Details Content`.
3. Delete everything inside `Details Content`.
4. Keep the empty `Details Content` frame.
5. Keep the bottom button.

## 6.3. Update the Bottom Button

1. Select `Button / Place Order`.
2. Rename it:

   ```text
   Button / Back to Menu
   ```

3. Change the text to:

   ```text
   Back to Menu
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

## 6.4. Create the Confirmation Icon

### Create the Check Mark

1. Press `T`.
2. Create a text layer inside `Details Content`.
3. Enter:

   ```text
   ✓
   ```

4. Rename it:

   ```text
   Check Mark
   ```

5. Apply:

   - Font: Inter
   - Weight: Semi Bold
   - Size: `60`
   - Fill: `Colour / Surface`
   - Text alignment: Centre

### Create the Circular Icon Frame

1. Select `Check Mark`.
2. Press `Shift + A`.
3. Rename the new frame:

   ```text
   Confirmation Icon
   ```

4. Configure it using:

   - Width: `120`
   - Height: `120`
   - Fill: `Colour / Success`
   - Corner radius: `999`
   - Horizontal alignment: **Centre**
   - Vertical alignment: **Centre**

Confirm that `Confirmation Icon` is nested inside `Details Content`.

## 6.5. Add the Confirmation Message

1. In `03 Order Summary`, select `Title + Subtitle`.
2. Copy it.
3. Select `Details Content` inside `04 Confirmation`.
4. Paste it underneath `Confirmation Icon`.
5. Change the title to:

   ```text
   Order Placed!
   ```

6. Change the subtitle to:

   ```text
   Your iced latte will be ready soon.
   ```

7. Centre the title and subtitle text.
8. Configure `Title + Subtitle` using:

   - Direction: **Vertical**
   - Gap: `8`
   - Alignment: **Centre**
   - Width: **Fill container**
   - Height: **Hug contents**

Keep:

- Title: `28` px Bold
- Subtitle: `14` px Regular
- Fill: `Colour / Text`

## 6.6. Configure Details Content

Select `Details Content` and apply:

- Direction: **Vertical**
- Gap: `24`
- Alignment: **Centre**
- Width: **Fill container**
- Height: **Hug contents**

Its hierarchy should be:

```text
Details Content
├── Confirmation Icon
│   └── Check Mark
└── Title + Subtitle
    ├── Title
    └── Subtitle
```

## 6.7. Adjust the Screen Padding

Select `04 Confirmation` and apply:

- Direction: **Vertical**
- Gap: **Auto**
- Alignment: **Top left**
- Horizontal padding: `24`
- Top padding: `96`
- Bottom padding: `48`

The increased top padding places the confirmation content lower on the screen while the automatic gap keeps `Button / Back to Menu` at the bottom.

The complete structure should be:

```text
04 Confirmation
├── Details Content
│   ├── Confirmation Icon
│   │   └── Check Mark
│   └── Title + Subtitle
│       ├── Title
│       └── Subtitle
└── Button / Back to Menu
```

## 6.8. Confirmation Screen Checkpoint

Your Confirmation screen should contain:

- [ ] A frame named `04 Confirmation`
- [ ] A `120 × 120` green confirmation icon
- [ ] A white `60` px Semi Bold check mark
- [ ] The title `Order Placed!`
- [ ] The subtitle `Your iced latte will be ready soon.`
- [ ] Centred confirmation text
- [ ] A top padding of `96`
- [ ] A full-width `Button / Back to Menu`
- [ ] Clearly named and nested layers

---

[Next: Section 7 – Connect and Test the Prototype](07-connect-and-test-the-prototype.md)
