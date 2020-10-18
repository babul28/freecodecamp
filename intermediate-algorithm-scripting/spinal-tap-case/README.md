# Intermediate Algorithm Scripting: `Spinal Tap Case`

Convert a string to spinal case. Spinal case is all-lowercase-words-joined-by-dashes.

## :point_right: Result

- `spinalCase("This Is Spinal Tap") should return "this-is-spinal-tap".`
- `spinalCase("thisIsSpinalTap") should return "this-is-spinal-tap".`
- `spinalCase("TheAndyGriffith_Show") should return "the-andy-griffith-show".`
- `spinalCase("Teletubbies say Eh-oh") should return "teletubbies-say-eh-oh".`
- `spinalCase("AllThe-small Things") should return "all-the-small-things".`

## Answer

```javascript
function spinalCase(str) {
  return str
    .split(/\s|_|(?=[A-Z])/) // split depends on white space, underscore, and before capital word
    .join('-')
    .toLowerCase();
}

spinalCase('This Is Spinal Tap');
```
