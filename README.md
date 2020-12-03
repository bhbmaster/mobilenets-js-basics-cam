# Simple Video Prediction with Mobilenet Tensorflow

Start liveserver (VSCode extension) or php:

    php -S localhost:1111

Then view from browser on localhost computer or over https on phone browser. If not localhost, must be https to get camera.

To get access over https use ngrok (install it if its missing):

    ngrok http <port>

Change <port> to match your http server port.
So with liveserver it should be 5500 by default, and with php we used 1111.

You will see output like this:

    Session Status                online                                                                                                                  
    Session Expires               7 hours, 53 minutes                                                                                                     
    Version                       2.3.35                                                                                                                  
    Region                        United States (us)                                                                                                      
    Web Interface                 http://127.0.0.1:4040                                                                                                   
    Forwarding                    http://e1d21550b36.ngrok.io -> http://localhost:5500                                                                   
    Forwarding                    https://e1d21550b36.ngrok.io -> http://localhost:5500

Ngrok will give you an http and https tunneled site. They can be accessed remotely and you will see your webserver.

* Open the https link from a remote browser to see the camera and prediction*

Cameras implemented using navigator.mediaDevices module only work over http if you are localhost (https locally too). If remote, you must use https.
