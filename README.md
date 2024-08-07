# IMAGE STEGANOGRAPHY
---

### Description
Developed a model that is very useful for data security.Here important data is image so it is necessary to secure thsis image before sending to anyone.so that our important data can't be seen by any other anonynomus user.It can only be seen after decryption to specified person.

### Technologies Used
- **Programming Language:** python
### Key Features
- **Data Security:**  encryption to ensure data privacy.
- **Efficient Data Retrieval:** decyption
  

### How It Works
1. **RETRIEVING A CONCATENATED STRING OF RGB CHANNEL VALUES OF ALL PIXELS OF SECRET IMAGE** : for this used BINARY BIT PLANE DECOMPOSITION ALGORITHM
2. **HIDING SECRET IMAGE IN SOURCE IMAGE:** used LSB steganography technique
3. **EXTRACT HIDDEN PIXELS** this one comes under decyption part to get backsecret image pixel from source image
4. **RECONSTRUCT IMAGE** after getting source image pixel we reconstruct original image

### Depiction of the proposed model 

***SOURCE IMAGE***


***![Pictures](https://github.com/mdshakebakhtar003/IMAGE-STEGANOGRAPHY/assets/160420527/750174ec-2bb0-4dfb-b68e-d115b72a10d0)***



***SECRET IMAGE***


***![Picturesec](https://github.com/mdshakebakhtar003/IMAGE-STEGANOGRAPHY/assets/160420527/6e3a699d-9997-4ec8-85f7-21305a136c02)***



***ENCRYPTED IMAGE***


***![Pictureen](https://github.com/mdshakebakhtar003/IMAGE-STEGANOGRAPHY/assets/160420527/e9b4945c-2ca3-4cc2-a8a6-0bd8eadb0843)***




***DECRYPTED IMAGE***


***![Picturedec](https://github.com/mdshakebakhtar003/IMAGE-STEGANOGRAPHY/assets/160420527/c6154b92-0683-46b4-bab2-140abc29399d)***






### CONCLUSION
In the encryption process, first we read the carrier image and original image from the file. Then perform the binary bitplane decomposition process for the both images. In binary bit plane decomposition, source and secret images are broken down into their binary components. After converting them into bit strings and RGB values, the last 4 bits  of the source image's RGB values are replaced with the  bits of the secret image, discretly embedding information while preserving the souce's visual integrity. This technique allows for covert communication or data transmission within digital images. By this the image is encrypted. Encrypted output for the image is obtained. Image decryption is performed in the reverse order of encryption. Thus the original image is obtained.
The source image should be more then double the size of the secret image. Since, we are taking 4 bits (half data of a pixel) of a pixel of secret image to replace it with 4 bits of a pixel of source image, and leave the RGB as it is, so to embed total data of secret image, source image’s size must be double of original image.
Our focus was to extract the secret image with minimum data loss, and we achieved that. However, the quality of our carrier image degraded.
