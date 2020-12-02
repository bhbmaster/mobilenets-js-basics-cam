# Simple Video Prediction with Mobilenet Tensorflow

Start liveserver (VSCode extension) or php:

    php -S localhost:1111

Then view from localhost browser or over https on phone browser (to get phone camera).

To get over https use ngrok (install it):

    ngrok http <port>

Change <port> to match the port liveserver or php maps to. For php most likely you used 1111 (but you could have used any), and for liveserver most likely it gave you 5500.

Example output will have lines like this:

    Session Status                online                                                                                                                  
    Session Expires               7 hours, 53 minutes                                                                                                     
    Version                       2.3.35                                                                                                                  
    Region                        United States (us)                                                                                                      
    Web Interface                 http://127.0.0.1:4040                                                                                                   
    Forwarding                    http://e1d21550b36.ngrok.io -> http://localhost:5500                                                                   
    Forwarding                    https://e1d21550b36.ngrok.io -> http://localhost:5500

Then when ngrok starts, it will give you an http and https tunneled site. Use the https one.

Cameras implemented with navigator.mediaDevices only work localhost or https.