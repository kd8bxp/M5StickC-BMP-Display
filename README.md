# M5StickC BMP Display

Finally, I was able to convert JPGs to an Array that the M5StickC likes.  

1) Convert your image to 16Bit color using this tool:  
    https://online-converting.com/image/convert2bmp/#  
    Select your 'Color' before you upload the picture to convert, you can also  
    change the picture size, if you want.  
    Select 16 (5:6:5, RGB Hi Color).  
    You will download a BMP image, this needs to be converted to a JPG.  
2) Convert and resize your image as needed, I used GIMP.  You can also rotate, but don't  
    change any color settings. Export to JPG.  
3) Now we need to convert the JPG to an Array. Use this tool https://littlevgl.com/image-to-c-array  
    I used 'True Color', and 'C array' for the settings. Upload your file, and click  
    Convert, download the array.  
4) The array should contain different color formats, you need to find the one that matches our settings.  
You will need to find the one marked '/*Pixel format: Red: 5 bit, Green: 6 bit, Blue: 5 bit*/' and copy everything between the #define and the #enddef   
If you copy the array and replace the array in one of the sketches, you should have a picture on your M5StickC.  

That's it.  

 Picture of Littlebits from Rick and Morty, Picture of one of the Grandkids (scaled pretty good), and a picture of the Planetary Union Emblem from The Orville.  

Have fun, and happy converting.  

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## Support Me

If you find this or any of my projects useful or enjoyable please support me.  
Anything I do get goes to buy more parts and make more/better projects.  
https://www.patreon.com/kd8bxp  
https://ko-fi.com/lfmiller  
https://www.paypal.me/KD8BXP  

## Other Projects

https://www.youtube.com/channel/UCP6Vh4hfyJF288MTaRAF36w  
https://kd8bxp.blogspot.com/  


## Credits

Copyright (c) 2020 LeRoy Miller

## License

This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses>
