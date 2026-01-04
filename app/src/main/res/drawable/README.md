# Drawable Resources

This folder contains shape drawables and vector drawable icons used by the Android XML components.

## Shape Drawables

### Basic Shapes
- **`shape_circle.xml`** - Circular shape for backgrounds, buttons, indicators
  - Can be tinted with `android:backgroundTint`
  - Used in: FloatingButton, AlphabeticalIndex, Checkbox/RadioButton backgrounds

### Form Control Shapes
- **`shape_checkbox_unselected.xml`** - Checkbox border (unselected state)
  - 20dp x 20dp circle with 2dp border
  - Border color: #888888
  - Used in: Checkbox component

- **`shape_checkbox_selected.xml`** - Checkbox background (selected state)
  - 20dp x 20dp filled circle
  - Background color: #008758 (green)
  - Used in: Checkbox component

- **`shape_radio_unselected.xml`** - Radio button border (unselected state)
  - 20dp x 20dp circle with 2dp border
  - Border color: #888888
  - Used in: RadioButton component

- **`shape_radio_selected.xml`** - Radio button border (selected state)
  - 20dp x 20dp circle with 2dp border
  - Border color: #008758 (green)
  - Used in: RadioButton component

### Progress Indicators
- **`progress_circular.xml`** - Circular progress indicator
  - Background: #D8D8D8
  - Progress: #2371EE (blue)
  - Note: For full functionality, may need custom view implementation
  - Used in: ProgressIndicatorCircular component

## Vector Drawable Icons

All icons are vector drawables converted from SVG source files.

### Form Icons
- **`ic_checkmark.xml`** - Checkmark icon (24dp)
  - Color: White (tinted in components)
  - Used in: Checkbox (selected state)

- **`ic_clear.xml`** - Clear/Close icon (24dp)
  - Color: Gray (#333333)
  - Used in: TextField, SearchField (clear button)

### Navigation Icons
- **`ic_alarm_active.xml`** - Alarm icon active state (24dp)
  - Color: Blue (#2371EE)
  - Used in: NavItemHorizontal, NavItemVertical (selected state)

- **`ic_alarm_inactive.xml`** - Alarm icon inactive state (24dp)
  - Color: Gray (#333333)
  - Used in: NavItemHorizontal, NavItemVertical (unselected state)

### Action Icons
- **`ic_search.xml`** - Search icon (24dp)
  - Color: Gray (#333333)
  - Used in: SearchField

- **`ic_star.xml`** - Star icon (10dp)
  - Color: Dark gray (#191919)
  - Used in: AlphabeticalIndex (favorites)

- **`ic_pen_new.xml`** - Pen/Edit icon (32dp)
  - Color: White
  - Used in: FloatingButton

## Usage Notes

1. **Tinting**: Most icons can be tinted using `android:tint` or `android:backgroundTint` attributes
2. **Sizing**: Icons are defined at their standard sizes but can be scaled via layout attributes
3. **Colors**: Default colors are set, but can be overridden with tint attributes
4. **Custom Views**: Some components (like circular progress) may require custom view implementation for full functionality

## Adding New Drawables

When adding new drawable resources:
1. Place shape drawables in this folder
2. Convert SVG icons to Android vector drawable format
3. Use descriptive names following the `ic_` or `shape_` prefix convention
4. Document usage in component XML files

