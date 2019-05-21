# Input

## Overview

`matInput` is a directive that allows native `<input>` and `<textarea>` elements to work with `<mat-form-field>`

## `<input>` and `<textarea>` attributes

All of the attributes that can be used with normal `<intput>` and `<textarea>` elements can be used on elements inside `<mat-form-field>` as well.  This includes Angular directives such as `ngModel` and `formControl`.

The only limitation is that the `type` attribute can only be one of the values supported by `matInput`.

## Supported `<intput>` types

The following input types can be used with `matInput`:

 - color
 - date
 - datetime-local
 - email
 - month
 - number
 - password
 - search
 - tel
 - text
 - time
 - url
 - week

## Form field features

There are a number of `<mat-form-field>` features that can be used with any `<input matInput>` or `<textarea matInput>`.  These include error messages, hint text, prefix & suffix, and themeing.  For additional information abotu these features, see the form field documentation.

## Placeholder

The placeholder is text shown when the `<mat-form-field>` label is floating but the input is empty.  It is used to give the user an additional hint about what they should type in the input.  The placeholder can be specified by setting `placeholder` attribute on the `<input>` or `<textarea>` element.  In some cases that `<mat-form-field>` may use the placeholder as the label (see the form field label documentation).

## Examples

<iframe src="https://stackblitz.com/angular/pbxvvngbexr?embed=1&file=app/input-form-example.ts&hideNavigation=1&view=preview" height="700" width="800"></iframe>
