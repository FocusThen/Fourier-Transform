# Fourier Transform

### Frequency in images
![ss1](https://user-images.githubusercontent.com/47830409/63842990-52035580-c98e-11e9-8d40-79f140917b4c.PNG)

### İmportant code
```sh
def ft_image(norm_image):
    f = np.fft.fft2(norm_image)
    fshift = np.fft.fftshift(f)
    frequency_tx = 20*np.log(np.abs(fshift))
    
    return frequency_tx
```
