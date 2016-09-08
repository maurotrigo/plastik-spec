# Plastik Spec

Plastik is a powerful way to represent forms and their output structure, both as JSON objects.

It allows you to define and build forms dinamically, since it's language agnostic (although it's heavily inspired by the HTML 5 form concepts). As mentioned before, both the form fields definition and their output are JSON objects.

## Basic structure

A Plastik form is an array of fields. Each field is represented by an object with the following general properties:

- **name:** string - required
- **type:** string - optional, defaults to "text"
- **domain:** string - optional, defaults to null
- **caption:** string - optional, defaults to the *name* property
- **placeholder:** string - optional, defaults to ""
- **required:** boolean - optional, defaults to *false*
- **multiple:** boolean - optional, defaults to *false*

There are also some properties that should be used only for certain field *types*:

- **options:** object - optional, defaults to null, used for *select* type fields
- **maxlength:** number - optional, defaults to 15000, used for *text* type fields
- **fields:** array - optional, null, used for *composite* type fields

This set of properties allows you to build a very flexible form **dinamically**, separating the input and output desired from the presentation of the form's inputs

## Field properties

### name

This property is required

### type

### domain

### caption

### placeholder

### required

### multiple

### options

### maxlength

## Field types

### text

### number

### select

### file

### media

### image

### geopoint

### composite

====

## Examples

