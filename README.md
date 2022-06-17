# PROYECT.U6
INTELI
from PIL import Image
from pytesseract import *

pytesseract.tesseract_cmd = r'C:\Users\Usuario\AppData\Local\Programs\Tesseract-OCR\tesseract.exe'

img = Image.open('image.png')

resultado = pytesseract.image_to_string(img)

print(resultado)
