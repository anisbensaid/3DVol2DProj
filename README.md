# 3DVol2DProj
###Forward Projections using Fourier Transform

The main file is FVR_main.m.

The tilt axis (pivot) in the following example is Y which means that the volume will be projected on the plane-XZ.
The variable angle is used to generate projections on half the space -90 to 90 (180 degrees) with 2 degrees separating each projection
```octave
%Tilt axis : in this case y axis
pivot = 'Y';
for angle = -90:2:90
```


Adding noise using the matlab function agwn (add gaussian white noise)

```octave
%adding noise using agwn function
NoisyProjectionY = awgn(projection,15,'measured'); 
```

