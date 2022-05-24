# import argparse
# import cv2
# from numpy import True_
# # print(cv2.__version__)

# def extractImages(pathIn, pathOut):
#     count = 1
#     vidcap = cv2.VideoCapture(pathIn)
#     success,image = vidcap.read()
#     success = True
#     while success:
#         vidcap.set(cv2.CAP_PROP_FPS,(30))                           #<<<<<<<<<<<< 30 img/sec
#         success,image = vidcap.read()
#         print ('Read a new frame: ', success)
#         cv2.imwrite( pathOut + "extract_%d.jpg" % count, image)    
#         count += 1

# if __name__=="__main__":
#     a = argparse.ArgumentParser()
#     a.add_argument("--pathIn", help="path to video")
#     a.add_argument("--pathOut", help="path to images")
#     args = a.parse_args()
#     print(args)
#     extractImages(args.pathIn, args.pathOut)
    
    
    
    
import cv2 
vidcap = cv2.VideoCapture('5-morn/date_5morn.mp4') 
def getFrame(sec): 
    vidcap.set(cv2.CAP_PROP_POS_MSEC,sec*1000) 
    ret,frame = vidcap.read() 
    # if ret: 
    #     cv2.imwrite("frame "+str(sec)+" sec.jpg", image)     # save frame as JPG file 
    return ret 
sec = 0 
frameRate = 1
success = getFrame(sec) 
while success: 
    sec = sec + frameRate 
    sec = round(sec, 2) 
    success = getFrame(sec) 
    print(success)
