# Chips

## Overview

`<mat-chip-list>` displays a list of values as individual, keyboard accessible, chips.

``` html
<mat-chip-list>
    <mat-chip>Papadum</mat-chip>
    <mat-chip>Naan</mat-chip>
    <mat-chip>Dal</mat-chip>
</mat-chip-list>
```

## Unstyled chips

By default `<mat-chip>` has Material Design styles applied.  For a chip with no styles applied, use `<mat-basic-chip>`.  You can then customize the chip appearance by adding your own CSS.

Hint: `<mat-basic-chip>` receives the `mat-basic-chip` CSS class in addition to the `mat-chip` class.

## Selection

Chips can be selected via the `selected` property.  Selection can be disabled by setting `selectable` to `false` on the `<mat-chip-list>`.

Whenever the selection state changes, a `ChipSelectionChange` event will be emitted via `(selectionChange)`.

## Disabled chips

Individual chips may be disabled by applying the `disabled` attribute to the chip.  When disabled, chips are neither selectable nor focusable.

## Chip Input

The `MatChipInput` directive can be used together with a chip-list to streamline the interaction between the two components.  This directive adds chip-specific behaviors to the input element within `<mat-form-field>` for adding and removing chips.  The `<input>` with `MatChipInput` can be placed inside or outside the chip-list element.

An example of chip input placed inside the chip-list element.

<iframe src="https://stackblitz.com/angular/klbapdmabak?embed=1&hideNavigation=1&view=preview" height="700" width="800"></iframe>

An example of chip input placed outside the chip-list element.

``` html
<mat-form-field>
  <mat-chip-list #chipList>
    <mat-chip>Chip 1</mat-chip>
    <mat-chip>Chip 2</mat-chip>
  </mat-chip-list>
  <input [matChipInputFor]="chipList">
</mat-form-field>
```

An example of chip input with an autocomplete placed inside the chip-list element.

<iframe src="https://stackblitz.com/angular/lmgnbmvdeopd?embed=1&file=app/chips-autocomplete-example.ts&hideNavigation=1&view=preview" height="700" width="800"></iframe>

## Themeing

The selected color of an `<mat-chip>` can be changed by using the `color` property.  By default, chips use a neurtral background color based on the current theme (light or dark).  This can be changed to `'primary'`, `'accent'`, or `'warn'`.

## Examples

<iframe src="https://stackblitz.com/angular/rxrqnovoxqk?embed=1&file=app/chips-overview-example.ts&hideNavigation=1&view=preview" height="700" width="800"></iframe>