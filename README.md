# Smallest valid image files

The purpose of this project is to find the smallest image file in various formats, which you can easily use as the default src value in the page before the img loads:

```html
<img src="data:image/jxl;base64,/wr6HwGRCAYBAFAASzhB5k11/Ia1kyog0AHeH0nCAVw">
```

Feel free to give me the smaller size files :)

## avif

```base64
AAAAHGZ0eXBhdmlmAAAAAGF2aWZtaWYxbWlhZgAAAOptZXRhAAAAAAAAACFoZGxyAAAAAAAAAABwaWN0AAAAAAAAAAAAAAAAAAAAAA5waXRtAAAAAAABAAAAImlsb2MAAAAAREAAAQABAAAAAAEOAAEAAAAAAAAAEgAAACNpaW5mAAAAAAABAAAAFWluZmUCAAAAAAEAAGF2MDEAAAAAamlwcnAAAABLaXBjbwAAABNjb2xybmNseAABAA0ABoAAAAAMYXYxQ4EgAgAAAAAUaXNwZQAAAAAAAAABAAAAAQAAABBwaXhpAAAAAAMICAgAAAAXaXBtYQAAAAAAAAABAAEEAYIDBAAAABptZGF0EgAKBzgABhAQ0GkyBRAAAAtA
```

Length: `288` bytes.

I created a 1x1 grey image using gimp and got this 288 bytes "nearly lossless" avif, I think it's the smallest.

## gif

```base64
R0lGODdhAQABAIABAICAgP///ywAAAAAAQABAAACAkQBADs
```

Length: `35` bytes.

## jpeg

```base64
/9j/4AAQSkZJRgABAQEASABIAAD/2wBDAP//////////////////////////////////////////////////////////////////////////////////////wgALCAABAAEBAREA/8QAFBABAAAAAAAAAAAAAAAAAAAAAP/aAAgBAQABPxA
```

Length: `134` bytes.

Taken from [stackoverflow](https://stackoverflow.com/questions/70033579/smallest-valid-base64-avif-image/77829744)

## jxl

```base64
/wr6HwGRCAYBAFAASzhB5k11/Ia1kyog0AHeH0nCAVw
```

Length: `32` bytes.

Taken from [stackoverflow](https://stackoverflow.com/questions/70033579/smallest-valid-base64-avif-image/77829744)

## png

```base64
iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAAAAAA6fptVAAAACklEQVQI12NoAAAAggCB3UNq9AAAAABJRU5ErkJggg
```

Length: `67` bytes.

## svg

```html
<svg xmlns='http://www.w3.org/2000/svg'></svg>
```
Length: `46` bytes.

svg file can get smaller data URI:

```html
<img src="data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg'%3e%3c/svg%3e">
```

## webp

```base64
UklGRh4AAABXRUJQVlA4TBEAAAAvAAAAAAdQwAIWsP+BiOh/AAA
```

Length: `38` bytes.
