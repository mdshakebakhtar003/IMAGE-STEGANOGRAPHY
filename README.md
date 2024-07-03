# IMAGE STEGANOGRAPHY
---
//## Client-Server Model with Socket Programming and AES-CBC Encryption

### Description
Developed a model that is very useful for data security.Here important data is image so it is necessary to secure thsis image before sending to anyone.so that our important data can't be seen by any other anonynomus user.It can only be seen after decryption to specified person.

### Technologies Used
- **Programming Language:** python
### Key Features
- **Data Security:**  encryption to ensure data privacy.
- **Efficient Data Retrieval:** decyption
- 

### How It Works
1. **RETRIEVING A CONCATENATED STRING OF RGB CHANNEL VALUES OF ALL PIXELS OF SECRET IMAGE** : for this used BINARY BIT PLANE DECOMPOSITION ALGORITHM
2. **HIDING SECRET IMAGE IN SOURCE IMAGE:** used LSB steganography technique
3. **EXTRACT HIDDEN PIXELS** this one comes decyption part to get backsecret image pixel from source image
4. **RECONSTRUCT IMAGE** after getting source image pixel we reconstruct original image

