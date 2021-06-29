# Multi-band Blending

A Python implementation of Multi-band Blending (also known as Laplacian Pyramid Blending).

## Dependencies

* Python 3.6+
* OpenCV 4.4.0

## Run

```
python multi_band_blending.py -f FIRST -s SECOND [-m MASK] -o OVERLAP [-S SIGMA] [-l LEVELS] [-H]

For example:
python multi_band_blending.py -f samples/l.jpg -s samples/r.jpg  -o 512
```

```
  -h, --help            show this help message and exit
  -f FIRST, --first FIRST
                        path to the first (left) image
  -s SECOND, --second SECOND
                        path to the second (right) image
  -m MASK,  --mask MASK    
                        path to the mask image
  -o OVERLAP, --overlap OVERLAP
                        width of the overlapped area between two images, even
                        number recommended
  -l LEVELS, --levels LEVELS
                        number of levels of multi-band blending, calculated
                        from image size if not provided
  -H, --half            option to blend the left half of the first image and
                        the right half of the second image
```

## References

https://github.com/cynricfu/multi-band-blending

OpenCV samples: opencv/samples/python/lappyr.py
