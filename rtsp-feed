import cv2
import numpy as np
import urllib.request as ur


while True:
    img_rtsp  = ur.urlopen ('http://192.168.43.1:8080/shot.jpg')
     
    img_re = np.array(bytearray(img_rtsp.read()), dtype = np.uint8)
     
    img_final = cv2.imdecode(img_re,-1)
     
    cv2.imshow("IPCAM",img_final)
     
    if cv2.waitKey(1)&0xFF == ord("q"):
        break
