## Define output filenames during multi image conversion

```
convert * -resize 1024x768 -quality 80 -density 72 \
          -set filename:f '%t_%wx%h.%e' \
          -set filename:dir '%wx%h' \
           '1024x768/%[filename:f]'
           
```

## High optimization of multiple images

```
convert * -resize 300x200  \
          -strip -interlace Plane -sampling-factor 4:2:0 -quality 90% -density 72 \ 
          -set filename:f '%t.%e' '300x200/%[filename:f]'
```