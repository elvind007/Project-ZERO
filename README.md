# PROJECT ZERO (AR application using Python)
- ## Configration
   - Anaconda Virtual Environment
   - python 3.7
   - Install external lib
        - First, you should install opencv and else libs in current directory
       ```
       pip install -r requirements.txt
       ```
        - Second, you should install opengl and pygame(which used to load textures) in your python environment. 
          Corresponding libs are in the [ExternalConfig] folder, you can copy them to your python environment and directly install
        ```
        python -m pip --user pygame-1.9.6-cp37-cp37m-win_amd64.whl
        ```
- ## Get camera information
  ### In the program, we need your camera information including intrinsic matrix and distortion coefficient and we use chessboard calibration to get it.
  - First, you should download a chessboard image, also provided for you in [ChessBoard] folder. After that, use the camera to capture at least 20 photos and save them to [ChessBoardSet] folder.
  - Second, execute [CameraCalibratioin.py] and you can find camera information in [CameraParameter/data1.txt]

- ## Run the program
  - First, copy the camera intrinsic matrix and distortion coefficient to replace corresponding paramaters [AR_entrance.py]
  - Second, run the [AR_entrance.py] and you can change models which are saved in [Models] directory.
  - Third, you can press **'+'** or **'-'** to scale the model size 
  
  - Note: you can generating the aruco mark by your self on [aruco generator](http://chev.me/arucogen/) (use 6x6 aruco)

  - **If you like it please give me a star and fork it :)**
  
