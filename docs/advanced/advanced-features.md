# Advanced Features

This section covers features intended for room administrators and power users.

---

## Managing Anchors

To manage Anchors for a room:

1. From the Portal, select **Rooms** → **Manage Rooms**
2. Select the room you want to modify
3. Click **Manage Anchors** from the operations menu

---

## Adding Additional Anchors

You can create multiple Anchors in a single room for more complex setups.

1. In the Manage Anchors dialog, click **Add Anchor**
2. Enter an Anchor name
3. Select an Anchor type (see below)
4. Confirm — then follow the standard steps to place and lock the new Anchor in XR

---

## Anchor Types

| Type | When to use |
|------|-------------|
| **Automatic** | Default. Use in most cases. The first Automatic Anchor in a room is designated "Center." Subsequent Automatic Anchors are shared between devices based on the Center Anchor's position. |
| **Manual** | Use if devices are struggling with automatic alignment, or for temporary setups where the Anchor position may change frequently. Must be placed individually per device and is not synced between users. |
| **Compound** | Advanced use only. Creates an Anchor centered between two existing Anchors. |

### Notes on Automatic Anchors

- Non-center Automatic Anchors can be moved by one user when unlocked, and changes sync to all devices in the room
- Non-center Automatic Anchor positions can also be adjusted numerically (in meters) from the Portal

---

## Updating an Individual Anchor

Select an Anchor from the list in the Manage Anchors dialog, then choose from the toolbar:

- **Edit** — update Anchor name or add it to a Local Anchor Group
- **Reset** — unlocks the Anchor for all users so it can be repositioned
    - *Not available for the Center Anchor*
    - All users in the room will need to reposition and re-lock after a reset
- **Delete** — removes the Anchor
    - All rooms must have at least one Anchor

---

## Refine Anchors

Use this when an Anchor is out of place on one device only (similar to Reposition in the Anchor Menu, but initiated from the Portal).

1. In XR, locate the misaligned Anchor and note its **4-letter Anchor Code**
2. In the Portal, enter that code where prompted in the Manage Anchors dialog
3. Click **Refine** — [App] will unlock the Anchor so it can be repositioned on that device

---

## Clear Room Map

This resets the spatial map that the Center Anchor's position is based on. **Use sparingly** — the Center Anchor is intended to be permanent.

Use only if:

- All devices are having trouble locating the Center Anchor, or
- The room's physical layout has significantly changed since initial setup

**What happens after clearing:**

- The next device to join the room will re-scan and re-place the Center Anchor for everyone
- Devices that previously bypassed alignment and placed manually may retain their old Anchor positions — adjust these individually via the Anchor Menu

!!! warning
    Clearing the room map affects all users. Coordinate with your team before doing this during an active session.
