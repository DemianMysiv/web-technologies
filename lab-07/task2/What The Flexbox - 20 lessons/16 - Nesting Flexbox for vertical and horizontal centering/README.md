# 14 — Nesting Flexbox (screenshots 121–137)

In the slider navigation, `ul` is the **outer flex container** and each `li` is a **flex item**. Once `li { display:flex }` is set, that same list item becomes an **inner flex container** for its anchor. The six list items have different flex factors: the two arrow elements get `flex:1`, the four text elements get `flex:2`. The anchor receives `flex-basis:100%`, `display:flex` and `align-items:center`; a nested span fills the full anchor width, providing centering. Red borders appeared in intermediate debugging states but are omitted from the final view.

The screenshot's illustration was a local `slide.jpeg` that was not uploaded as a standalone asset. The HTML retains the referenced filename; the exact picture is therefore absent. Add your own image at `slide.jpeg` to display it.

`examples/` contains eight course-progress snapshots, not distinct complete websites. Open `index.html` with `style.css` for final layout.
