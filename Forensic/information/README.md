Question :

![alt text](https://github.com/MrPayMac/picoCTF/blob/main/Forensic/information/Question.png?raw=true)

Hints1
![alt text](https://github.com/MrPayMac/picoCTF/blob/main/Forensic/information/Hints1.png?raw=true)

Hints2
![alt text](https://github.com/MrPayMac/picoCTF/blob/main/Forensic/information/Hints2.png?raw=true)

1. Use `exiftool cat.jpg`
2. copy the License = `"cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9"`
3. type `echo "cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9" | base64 -d`

Flag = `picoCTF{them3tadata_1s_modified}`
