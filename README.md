# Detect Real-time hand gestures  
**Examples are in the directory and demonstrated in the python notebook!**  

## **Using OpenCV, Tensorflow, and LSTM to detect hand gestures in real-time**

## Start:  

You need to have a camera connected to your machine and functioning correctly

### Create virtual environment:   
```python -m venv myenv```
### activate the environment:   
```source myenv/bin/activate```

## Notice:
-I used a pip mirror in China since I am travelling, but you don't have to
Simply change the pip install line to:  
```!pip install tensorflow==2.8.1 tensorflow-gpu==2.8.1 opencv-python mediapipe scikit-learn matplotlib```   

-The gpu option is disabled since I am away from my computer that can run models with gpu. I encourage you to try to turn it on since it is alot faster to train. 

-The gestures I tried to classify are hello, no, and iloveyou. However, you can modify the # of class in:  
```# Actions that we try to detect```  
```actions = np.array(['hello', 'no', 'iloveyou'])```

You can adjust the # of training samples here:  
```# Thirty videos worth of data```  
```no_sequences = 30```  


Remember to clear the memory and free up the camera once you stop the training process by:

```cap.release()```  
```cv2.destroyAllWindows()```    
