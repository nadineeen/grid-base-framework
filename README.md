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

## Containers

This framework comes with two different containers:

- `.container` which `width: 100%` regardless of screen width
- `.container-{breakpoint}` which is `width: 100%` until the specified breakpoint.

After they reach their specify breakpoint, the containers will change at each higher breakpoint to be 97% of that breakpoint.

## Columns

This framework comes with two different columns:

- `.col-{n}` where 1 < n < 12 which determines how many 'cells' a column should span regardless of the screen width
- `.col-{breakpoint}-{n}` where the column's width is 100% until the specified breakpoint
