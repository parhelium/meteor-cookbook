## Define output filenames during multi image conversion

```
convert * -resize 1024x768 -quality 80 -density 72 \
          -set filename:f '%t_%wx%h.%e' \
          -set filename:dir '%wx%h' \
           '1024x768/%[filename:f]'
           
```