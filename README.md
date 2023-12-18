# Form standard tests

This is a guide for testing forms in web applications.

<br />

## General

- accept empty value
- is hidden field
- is required
- is unique value

<br />

## Index field

**UUID**
- is valid uuid format

**Slug**
- is valid slug format

<br />

## Numeric field

**Boolean**
- accepts false
- accepts indeterminate
- accepts true

**Number**
- accepts decimal numbers
- accepts integer numbers
- accepts limited number of decimal digits
- accepts limited number of integer digits
- accepts negative numbers
- accepts number in range
- accepts positive numbers
- accepts zero
- does not accept letters
- does not accept numbers with leading zeros
- does not accept only decimal digits
- does not accept only spaces
- does not accept scientific notation
- does not accept special characters
- does not auto complete value

<br />

## Text field
- accepts leading spaces
- accepts trailing spaces
- accepts intermediate spaces
- accepts line breaks
- accepts numbers
- accepts another language characters
- accepts letters with diacritics
- accepts limited number of characters
- accepts lowercase letters
- accepts uppercase letters
- accepts special characters
- accepts emojis
- does not accept invisible characters
- does not accept only spaces
- does not auto complete value
- XSS protection

**CSRF token**
- is valid csrf token format

**Email**
- is valid email format

**File path**
- is valid file path format

**JSON**
- is valid json format

**Password**
- is valid password format

**Telephone number**
- is valid telephone number format

**URL**
- is valid url format
- accepts HTTP and HTTPS protocols
- does not accept any protocols but HTTP and HTTPS

<br />

## Select and radio field
- accepts a value in valid choices
- accepts multiple values in valid choices if the field is multiple
- does not accept a value that is not in valid choices
- has an disabled default option

<br />

## Date or Time field
- accepts earlier date or time
- accept later date or time
- accepts current date or time

**Date**
- is valid ISO 8601 date format

**Datetime**
- is valid datetime format

**Duration**
- is valid duration format

**Time**
- is valid time format

<br />

## File field
- accepts any file name
- accepts files with valid file size
- accepts files with valid file type
- XSS protection

**CSV**
- is valid csv format with headers
- is valid csv format without headers
- is valid data
- is valid data structure

**Image**
- accepts images with valid dimensions
- accepts images with valid file type

<br />

## Formsets

**After submit**

- create saved new items
- delete non saved existing items
- update saved existing items

**Existing items**

- remove an existing item
- shows existing items in correct order
- shows existing items with correct values
- update value in existing item

**New items**

- create a new item
- remove a new item
- shows new items in correct order
- update value in new item
