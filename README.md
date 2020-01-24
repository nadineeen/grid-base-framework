# grid-base-framework

Custom 12 grid-base responsive framework

## Breakpoints

The breakpoint values for this responsive framework are:
| Breakpoint | Size |
| ---------- | :----: |
| xs | 375px |
| s | 667px |
| m | 768px |
| l | 1024px |
| xl | 1200px |

(These values are located in the `_breakpoints.scss` file and can be changed to your liking)

## Containers

This framework comes with two different containers:

- `.container` which `width: 100%` regardless of screen width
- `.container-{breakpoint}` which is `width: 100%` until the specified breakpoint.

After they reach their specify breakpoint, the containers will change at each higher breakpoint to be 97% of that breakpoint.

## Rows

This framework comes with two different rows. All of them are flex boxes.

- `.row` which is a flex box with a flex direction of row with no fixed height
- `.row-{n}` where 1 < n 12 which has a fixed height of 100\*n pixels

## Columns

This framework comes with three different columns:

- `.col` which is a flex box with a flex direction of column with no fixed width
- `.col-{n}` where 1 < n < 12 which determines how many 'cells' a column should span regardless of the screen width
- `.col-{breakpoint}-{n}` where the column's width is 100% until the specified breakpoint

## Display from/until breakpoint

There are two ways of specifying when an element should display

- `.display-from-{breakpoint}`: element is displayed only from the specified breakpoint onwards
- `.display-until-{breakpoint}`: element is display up until the breakpoint specified

## Elements that fully cover the screen

The `.full-cover-{direction}` can be added to elements which allow them to take up the full height & width of the window screen. This can be used for full screen menus for example.

Initially, elements with `.full-cover-{direction}` are hidden (`width: 0` or `height: 0`). Thus to make them visible, the element must have the class `.active` as well.

There are four directions from which the element can appear (transition) from:

- `.full-cover-top` where element appears from the top downwards.
- `.full-cover-btm` where element appears from the bottom.
- `.full-cover-l` where element appears from the left.
- `.full-cover-r` where element appears from the right.

---

## Miscs

By default, `li`s' in `nav` elements have property `list-style: none`.

There are classes for text-alignment: `.ta-cnr` (center), `.ta-l` (left), `.ta-r` (right), `.ta-j`(justify).

There are some classes for flex properties for `.row` & `.col`:

- flex-wrap: `.nowrap` (nowrap)
- justify-content: `.jc-c` (center), `.jc-sb` (space-between)
