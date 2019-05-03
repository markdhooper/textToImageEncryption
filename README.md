# textToImageEncryption
Convert plain-text to an image and combine with additional images (private and public) to share with others in a public forum. The image can then be decrypted provided one has both images (private and public) to obtain the plain-text.

Video Demonstration:  https://www.youtube.com/watch?v=IdLkFhk0hmE

How to use: 

These scripts use Pillow to manipulate/create the necessary images.
Install Pillow:   https://pillow.readthedocs.io/en/stable/index.html 

1.  Create a text file named msg.txt. Put your secret message inside. (keep it under 1024 characters to be safe.)
2.  Run asciiToImage.py to create an image named msgImg.png.
3.  Run privateKeyGenerator.py to generate a randomly generated private key image called pk.png.
4.  Find an image of your liking and save it as pub.png.
5.  Run encrypt.py to generate eng.png (your encrypted image!).
6.  To decrypt you need to have both the private and public images that were used to make the original encrypted image in the same folder as the decrypt.py script. Run decrypt.py and you will find the original plain-text message in a file called decryptedMessage.txt.

* I plan to clean up the code and combine all things into one file for encryption. And minimise the number of diagnostic files created.
* you can use the script getRandomImages.py to obtain random pictures from picsum.com and save them as pub.png and pk.png.
