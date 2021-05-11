---
layout: post
title:      "Ghost Server Sighting"
date:       2021-04-25 16:48:32 -0400
permalink:  my_fellow_windows_users_in_a_react_framework
---

To my fellow Window users in a React framework... 

Scenario: You are drowning in React Labs and have too many Visual Studio Code Tabs open (like me) and come across a ghost server—a server still haunting the network not allowing you to launch a new one.  How do you find it and "kill" it? 

Earlier in the curriculum I used to restart my computer to kill the ghost server. Yeah…I did that! That soon ended when I was pair programming on zoom and I told my partner, “BRB, I need to hop off and restart my computer to kill this ghost server,” she said, “why do you need to restart your computer? We are software engineers, let’s figure this out!!”

Now here we are…to kill a ghost server on a Windows in a React App type this in your terminal:                         
                                                                       ```
																																			 npx kill-port <port number>
																																			 ```
																																			 

For example, I am currently running a localhost:3000 that I need to kill so I can start a new server. In the terminal I will type:

																											                        ```
																																							npx kill-port 3000
																																							````


And there you have it! I’d like to thank my pair program partner to inspire me to search for this random valuable information and Google for presenting it to me.  

