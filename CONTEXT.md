# Mini Games

This context defines player-facing language for the web games collection.

## Language

**Mobile Tetris controls**:
The touch-screen control set for Tetris. It includes left, right, down, rotate, and Hold controls, and is intentionally smaller than the desktop keyboard control set.
_Avoid_: Full keyboard controls, hard-drop-first controls

**Mobile down control**:
The down control in Mobile Tetris controls. A tap moves the active piece down by one row, while a long press repeatedly soft-drops it until released or until normal lock timing takes over.
_Avoid_: Hidden hard drop, instant lock

**Mobile hard drop**:
Mobile Tetris does not expose hard drop as a touch-screen action. Hard drop remains a desktop keyboard action.
_Avoid_: Hard drop button, hard drop gesture

**Mobile Tetris information panel**:
The compact right-side status area for mobile Tetris. It uses English labels and shows one Next piece, the Hold piece, Score, Lines, Level, and a small pause entry.
_Avoid_: Desktop stats panel, full Next queue

**Mobile play layout**:
The portrait mobile arrangement for Tetris. It places the board on the left, the Mobile Tetris information panel on the right, and movement/action controls along the bottom without covering the board.
_Avoid_: Centered-board mobile layout, desktop column stack

**Mobile landscape fallback**:
The touch-screen landscape arrangement for Tetris. It only needs to remain playable and should not drive the portrait mobile design.
_Avoid_: Portrait redesign scope, reference-image layout

**Mobile preview stack**:
The preview area inside the Mobile Tetris information panel. It places the single Next piece above the Hold piece.
_Avoid_: Side-by-side previews, full Next queue

**Mobile Hold control**:
The Hold control in Mobile Tetris controls. Its action button sits with the rotation control, while its piece preview belongs with the Next preview.
_Avoid_: Hidden Hold gesture, separate bottom Hold cluster

**Mobile action controls**:
The bottom-right action pair in Mobile Tetris controls. It places Hold and rotate side by side, separate from the left, down, and right movement controls.
_Avoid_: Hard drop button, pause button, stacked action column

**Mobile movement controls**:
The bottom-left movement trio in Mobile Tetris controls. It places left, down, and right in a single horizontal row.
_Avoid_: Direction pad, hard drop control

**Mobile pause entry**:
The pause control for mobile Tetris. It belongs with the information panel rather than the piece movement controls.
_Avoid_: Bottom pause button, movement control

## Example Dialogue

Developer: Should mobile Tetris mirror every keyboard action?

Domain expert: No. Mobile Tetris controls should stay compact: left, right, down, rotate, and Hold.

Developer: Should the mobile status area include Best score and Combo Max?

Domain expert: No. The mobile Tetris information panel should show one Next piece, the Hold piece, Score, Lines, Level, and pause, using English labels.

Developer: Should portrait mobile keep the board centered above stacked panels?

Domain expert: No. The Mobile play layout places the board on the left and the information panel on the right.

Developer: Should this portrait mobile redesign also define mobile landscape?

Domain expert: No. Mobile landscape fallback only needs to remain playable.

Developer: Should Next and Hold previews sit side by side?

Domain expert: No. The Mobile preview stack places Next above Hold.

Developer: Should holding down on mobile instantly hard-drop and lock the piece?

Domain expert: No. The Mobile down control is a repeat soft drop, not a hidden hard drop.

Developer: Should mobile include any separate hard drop action?

Domain expert: No. Mobile hard drop is intentionally absent.

Developer: Is pause one of the bottom movement controls on mobile?

Domain expert: No. The Mobile pause entry belongs in the information panel.

Developer: Where does Mobile Hold belong?

Domain expert: The Mobile Hold control button sits with rotate, and the Hold preview sits with Next.

Developer: Should Hold and rotate be stacked vertically on mobile?

Domain expert: No. Mobile action controls place Hold and rotate side by side.
