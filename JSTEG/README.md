# JSTEG
Jsteg is a package for hiding data inside JPEG files with a technique known as steganography. This is accomplished by copying each bit of the data into the least-significant bits (LSB) of the image. The amount of data that can be hidden depends on the file size of the jpeg; it takes about 10-14 bytes of jpeg to store each byte of the hidden data.

## Installation of JSTEG

`sudo wget -O /usr/bin/jsteg https://github.com/lukechampine/jsteg/releases/download/v0.1.0/jsteg-linux-amd64`

![image](https://github.com/KVNuhman/Steganography/assets/46161259/e986b813-022f-46be-becc-c550dbe6a803)

`sudo chmod +x /usr/bin/jsteg`

`sudo wget -O /usr/bin/slink https://github.com/lukechampine/jsteg/releases/download/v0.2.0/slink-linux-amd64`

![image](https://github.com/KVNuhman/Steganography/assets/46161259/16a24d73-c9ce-4efc-9498-e712e15f7627)

`chmod +x /usr/bin/slink`

## Usage

### Prerequisites

Create a sample txt file which contains the secret message which is to be embeded with the image.

![image](https://github.com/KVNuhman/Steganography/assets/46161259/9a3d5d25-8965-4f26-aea5-522709a9c3b1)

Download an image of any format and store it in the current directory `cover.jpg`.

### Embeding a File in a JPEG image

`jsteg hide <in.jpg> <secret file name> <out.jpg>`
`in.jpg` is our original file, `<secret file name>` is the name of text file and `out.jpg` is name of modified image file.

![image](https://github.com/KVNuhman/Steganography/assets/46161259/1ba3d4ba-ce03-47c3-a875-63544ccc9aad)

### Extracting the secret text

`jsteg reveal <in.jpg> <output file name>`

![image](https://github.com/KVNuhman/Steganography/assets/46161259/b7c024e6-5a0f-494c-84b5-36e58ded2307)








