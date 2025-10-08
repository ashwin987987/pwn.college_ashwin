# writeup
As the challenge talks about Metadata we first run exiftool on the image.
we get a big hint - kdj had a habit of hiding images within images. this clearly means a image is hidden within this image. We can extract the embedded image using foremost or binwalk.

Here we run foremost on challenge.jpg to extract the hidden image within the file. Alternatively we can also use binwalk on the terminal or its online alternative
This gives us the embedded PNG which gives us the flag.
# flag :
citadel{th1s_ch4ll3ng3_1s_f0r_th4t_0n3_ex1ft00l_4nd_b1nw4lk_enthus14st} 
