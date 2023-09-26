# PYTHON-QRCODE
this is basic code to make a QR
import qrcode as qr
from PIL import Image
q=qr.QRCode(version=1,error_correction=qr.constants.ERROR_CORRECT_H,box_size=10,border=4,) # .QRCode is used to change physical 
q.make("https://www.youtube.com/watch?v=5mvCVJIZWtA")                                #properties of a qr and it's error correction
img=q.make_image(fill_color="green",back_color="blue")
img.save("qrcode.png")
