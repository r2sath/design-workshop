# 7. Connect and Test the Prototype

The four screens currently show what the café app could look like, but they are not interactive yet.

In this section, you will connect the screens, set the starting point, present the prototype, and test the complete user flow.

## 7.1. Review the Required Flow

Create the following prototype connections:

| Starting Screen | Interactive Layer | Destination |
|---|---|---|
| `01 Menu` | `Button / View Item` inside `Card / Iced Latte` | `02 Item Details` |
| `02 Item Details` | `Button / Back` | `01 Menu` |
| `02 Item Details` | `Button / Add to Order` | `03 Order Summary` |
| `03 Order Summary` | `Button / Place Order` | `04 Confirmation` |
| `04 Confirmation` | `Button / Back to Menu` | `01 Menu` |

Use the same settings for every connection:

- Trigger: **On click**
- Action: **Navigate to**
- Transition: **Instant** or no animation

Only the Iced Latte `View Item` button is connected. The Blueberry Muffin and Grilled Cheese buttons remain non-interactive.

## 7.2. Open the Prototype Controls

1. Make sure none of the four screens are hidden or locked.
2. Open the **Prototype** controls in the right sidebar.
3. Keep the screens arranged from left to right:

   ```text
   01 Menu
   02 Item Details
   03 Order Summary
   04 Confirmation
   ```

This arrangement makes the connections easier to see and follow.

## 7.3. Set the Starting Point

The prototype should begin on the Menu screen.

1. Select `01 Menu`.
2. In the Prototype controls, set the frame as the flow starting point.
3. Confirm that a starting-point icon appears beside `01 Menu`.

Figma may name the flow `Flow 1`. The flow name can remain unchanged.

## 7.4. Connect the View Item Button

The `View Item` button inside the Iced Latte card opens the Item Details screen. The rest of the card remains non-interactive.

1. Expand `Card / Iced Latte` inside `01 Menu`.
2. Select `Button / View Item`.
3. Confirm that the **button frame**, rather than its text layer or the surrounding card, is selected.
4. Drag the prototype connection handle from `Button / View Item` to `02 Item Details`.
5. Configure:

   - Trigger: **On click**
   - Action: **Navigate to**
   - Destination: `02 Item Details`
   - Transition: **Instant** or no animation

## 7.5. Connect the Back Button

1. Select `Button / Back` inside `02 Item Details`.
2. Drag its prototype connection handle to `01 Menu`.
3. Configure:

   - Trigger: **On click**
   - Action: **Navigate to**
   - Destination: `01 Menu`
   - Transition: **Instant** or no animation

This creates a separate path that allows the user to return without adding the item to an order.

## 7.6. Connect Add to Order

1. Select `Button / Add to Order` inside `02 Item Details`.
2. Drag its connection handle to `03 Order Summary`.
3. Configure:

   - Trigger: **On click**
   - Action: **Navigate to**
   - Destination: `03 Order Summary`
   - Transition: **Instant** or no animation

## 7.7. Connect Place Order

1. Select `Button / Place Order` inside `03 Order Summary`.
2. Drag its connection handle to `04 Confirmation`.
3. Configure:

   - Trigger: **On click**
   - Action: **Navigate to**
   - Destination: `04 Confirmation`
   - Transition: **Instant** or no animation

## 7.8. Connect Back to Menu

1. Select `Button / Back to Menu` inside `04 Confirmation`.
2. Drag its connection handle to `01 Menu`.
3. Configure:

   - Trigger: **On click**
   - Action: **Navigate to**
   - Destination: `01 Menu`
   - Transition: **Instant** or no animation

This closes the loop and allows the prototype to begin again.

## 7.9. Review the Prototype Connections

The completed primary flow should be:

```text
01 Menu
→ View Item
→ 02 Item Details
→ Add to Order
→ 03 Order Summary
→ Place Order
→ 04 Confirmation
→ Back to Menu
→ 01 Menu
```

The separate Back-button path should be:

```text
02 Item Details
→ Back
→ 01 Menu
```

Confirm that:

- `Button / View Item` on the Iced Latte card opens Item Details.
- Clicking elsewhere on the Iced Latte card does not navigate.
- The Back button returns to the Menu.
- Add to Order opens the Order Summary.
- Place Order opens the Confirmation screen.
- Back to Menu restarts the flow.
- The Blueberry Muffin and Grilled Cheese buttons do not navigate.

## 7.10. Present and Test the Prototype

1. Click the **Present** or **Play** button near the top-right corner of Figma.
2. Confirm that the prototype opens on `01 Menu`.
3. Complete the main flow:

   1. Click `View Item` on the Iced Latte card.
   2. Click `Add to Order`.
   3. Click `Place Order`.
   4. Click `Back to Menu`.

4. Confirm that each button opens the correct screen.
5. Return to Item Details and test the `< Back` button separately.

## 7.11. Test with a Partner

Ask a partner to use the prototype without explaining what to click.

Observe whether they can:

- Identify how to view the Iced Latte.
- Understand what the Back button does.
- Add the item to the order.
- Review and place the order.
- Recognize that the order was successful.
- Return to the Menu.

Ask:

- Was the next action clear on every screen?
- Did any element look clickable when it was not?
- Did any button label feel confusing?
- Was any text difficult to read?
- Did the flow behave as expected?

Record any useful feedback and make small improvements if time allows.

## 7.12. Final Checklist

Before finishing, confirm that:

- [ ] All four screens are present and correctly named.
- [ ] `01 Menu` is the flow starting point.
- [ ] The Iced Latte `Button / View Item` opens `02 Item Details`.
- [ ] The card itself is not interactive.
- [ ] `Button / Back` returns to `01 Menu`.
- [ ] `Button / Add to Order` opens `03 Order Summary`.
- [ ] `Button / Place Order` opens `04 Confirmation`.
- [ ] `Button / Back to Menu` returns to `01 Menu`.
- [ ] The prototype can complete the full loop.
- [ ] The Blueberry Muffin and Grilled Cheese buttons remain non-interactive.
- [ ] Important frames and layers have clear names.
- [ ] Text is readable and does not overlap.
- [ ] Colours and spacing are consistent.

## 7.13. What You Created

You created an **interactive interface prototype**. It demonstrates:

- What the café app could look like.
- What information appears on each screen.
- Which controls the user can select.
- How the user moves through the ordering flow.

The prototype does not process payments, save an order, or communicate with a real café. Those behaviours would require software development beyond the interface design created in Figma.
