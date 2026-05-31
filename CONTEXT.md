# Mini Games

This context defines player-facing language for the web games collection.

## Language

**Mobile Tetris controls**:
The touch-screen control set for Tetris. It includes left, right, down, hard drop, Hold, and rotate controls, and is intentionally smaller than the desktop keyboard control set.
_Avoid_: Full keyboard controls, hidden gesture controls

**Mobile down control**:
The down control in Mobile Tetris controls. A tap moves the active piece down by one row, while a long press repeatedly soft-drops it until released or until normal lock timing takes over.
_Avoid_: Hidden hard drop, instant lock

**Mobile hard drop**:
The dedicated hard drop button in Mobile Tetris controls. It uses the former bottom action position beside the Hold/rotate stack.
_Avoid_: Hidden hard drop gesture, replacing the down control

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
The Hold control in Mobile Tetris controls. Its action button sits above the rotation control, while its piece preview belongs with the Next preview.
_Avoid_: Hidden Hold gesture, side-by-side Hold and rotate pair

**Mobile action controls**:
The bottom-right action cluster in Mobile Tetris controls. It places hard drop in the former Hold position, with Hold stacked above rotate beside it.
_Avoid_: Pause button, side-by-side Hold and rotate pair

**Mobile movement controls**:
The bottom-left movement trio in Mobile Tetris controls. It places left, down, and right in a single horizontal row.
_Avoid_: Direction pad, replacing down with hard drop

**Mobile pause entry**:
The pause control for mobile Tetris. It belongs with the information panel rather than the piece movement controls.
_Avoid_: Bottom pause button, movement control

## Example Dialogue

Developer: Should mobile Tetris mirror every keyboard action?

Domain expert: No. Mobile Tetris controls should stay compact: left, right, down, hard drop, Hold, and rotate.

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

Developer: Should mobile include a separate hard drop action?

Domain expert: Yes. Mobile hard drop is a dedicated bottom action button, not a down-button gesture.

Developer: Is pause one of the bottom movement controls on mobile?

Domain expert: No. The Mobile pause entry belongs in the information panel.

Developer: Where does Mobile Hold belong?

Domain expert: The Mobile Hold control button sits above rotate, and the Hold preview sits with Next.

Developer: Should Hold and rotate be stacked vertically on mobile?

Domain expert: Yes. Mobile action controls place Hold above rotate, with hard drop beside that stack.
