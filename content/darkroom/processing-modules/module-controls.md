---
title: module controls
id: module-controls
weight: 40
draft: false
---

This section describes how to interact with processing module controls.

# sliders

Sliders offer five different methods of interaction, depending on the level of control you require.

left-click (set)
: Click anywhere in the slider area to set the value. You can also click and drag to change it. You don't have to aim for the triangle or even the line -- you can click anywhere in the entire height of the slider, including the label.

mouse wheel (adjust)
: Hover over the slider with your mouse, then use your mouse wheel to adjust the value. You can alter the default speed at which the mouse scroll adjusts a slider by scrolling over that slider while in [visual shortcut mapping mode](../../preferences-settings/shortcuts.md#visual-shortcut-mapping).

keyboard arrow keys (adjust)
: When the slider has focus you can hover over the slider with your mouse, then use your keyboard's arrow keys (←/↓ and →/↑) to adjust the value. In order to give focus to the widget without changing the current value you can right-click, then right-click again.

right-click (pop-up edit)
: When your mouse is over a slider right-clicking enables a multi-functional pop-up below the slider for fine control with your mouse or numerical entry using the keyboard.

: ![bauhaus](./module-controls/bauhaus.png#w33)

: A bent line extending from the triangular marker moves with your mouse. The closer your mouse pointer is to the triangular marker the coarser the control you have over the value; the further away from the triangular marker the finer your control. Left-click with your mouse to accept the new value and hide the pop-up.

: Alternatively you can type in a new value using your keyboard and commit by hitting the Enter key. You may even supply the new value in the form of an arithmetic expression which darktable will calculate for you -- the previous value is referenced as “x”.

: For most sliders, the minimum and maximum values displayed are known as "soft limits" -- they do not represent the minimum/maximum values that you may enter, merely a suggested range of "normal" values that most users will not need to exceed. As well as these soft limits, each slider also has "hard limits" which may not be exceeded.

: You may right-click and type any value up to the hard limits for a given slider. For example, in the [_rotate and perspective_](../../module-reference/processing-modules/rotate-perspective.md) module, the soft limits for angle are -10 to +10 degrees while the hard limits are -180 to +180 degrees; In the [_exposure_](../../module-reference/processing-modules/exposure.md) module, the soft limits for the exposure slider are -3 to +4 EV while the hard limits are -18 to +18 EV. If you try to enter a value beyond the hard limit, it will be automatically be adjusted to the minimum/maximum allowable value.

double-click (reset)
: Double-click on a slider or its label to reset back to the default value. Ctrl+double-click to reset its value back to any auto-applied preset (if one applies for the current image). If controls are grouped together within a tabbed interface, you can double-click on the tab's header label to reset all settings in that tab.

In addition, the speed of mouse-wheel, arrow-key and click+drag adjustments can be altered:

 - hold down the Shift key while adjusting to _increase_ the step size by a factor of 10. 
 - hold down the Ctrl key while adjusting to _decrease_ the step size by a factor of 10.

Both of these multipliers can be amended in [preferences > shortcuts](../../preferences-settings/shortcuts.md) by altering the speed of the fallbacks/value actions.

# comboboxes

Click on a combobox to show a list of available options which you can click to select. Occasionally the selection list will open close to the bottom or top of the screen meaning that only some of the items are visible -- simply scroll with your mouse wheel to bring up the full list. Alternatively, you can also use the mouse wheel and keyboard arrow keys to select an option, or start typing to filter the combobox entries.

As with sliders, you can double-click the combobox or its label to reset back to the default value, or Ctrl+double-click to reset back to any auto-applied preset.

# pickers

Many modules allow parameters to be set using pickers (identified by the ![picker-icon](./module-controls/color-picker.png#icon) icon). Pickers allow you to select sample areas of the image from which to calculate values for module parameters. You can usually choose to select either a "point" (a single pixel) or an "area" (a rectangular selection of pixels) from the image, although some modules only allow one mode to be used.

Selecting pixel(s) will cause the appropriate module value(s) to be updated, and may also cause additional visual feedback (for example, overlaying the range of selected pixels on a tone curve).

Activate point mode by left-clicking the picker icon and then left-click anywhere on the image to select the pixel from which to calculate values. The selected point will be shown on-screen (with a cross icon) which you can adjust by left-clicking another pixel. Deactivate the picker by left-clicking the picker icon again.

Activate area mode by either right-clicking or Ctrl+clicking the picker icon and then left-click and drag to select a rectangular area of the image from which to calculate values. The selected area will be shown on-screen as an overlaid rectangle which can be moved by either drawing another rectangle elsewhere or by left-clicking and dragging the corners of the drawn rectangle. Reset the rectangle (to select the whole image) by right-clicking anywhere on the image. Deactivate the picker by right-clicking (or Ctrl+clicking) the picker icon again.

In modules where only one mode is available, left-clicking the icon will usually toggle that mode on and off.

# keyboard shortcuts

Module parameters can also be adjusted using keyboard shortcuts. See [preferences > shortcuts](../../preferences-settings/shortcuts.md) for more information.
