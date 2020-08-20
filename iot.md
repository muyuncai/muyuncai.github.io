---
layout: default
title: IOT
---
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>JSON Test</title>
</head>
<body>
    <ul id='json'>
    </ul>
    <!-- <script type="text/javascript" src="roomTemp.json></script>
    <script type="text/javascript" src="javascrip.js"></script> 
These should explain what was done: https://www.w3schools.com/jsref/prop_html_innerhtml.asp
https://www.w3schools.com/jsref/met_node_appendchild.asp
-->
    <script type='text/javascript'>
     const jsonData = [
        {
            "id": "1",
            "roomName": " Pet's Room",
            "temperature": " 22 Celsius"
        },
        {
            "id": "2",
            "roomName": " Bedroom",
            "temperature": " 24 Celsius"
        }
    ];

    jsonData.map((data) => {
        let node = document.createElement("LI");
        let element = document.createTextNode(data.id);        
        node.appendChild(element);
        element = document.createTextNode(data.roomName);
        node.appendChild(element); 
        element = document.createTextNode(data.temperature);
        node.appendChild(element); 
        document.getElementById('json').appendChild(node);
    })
    </script>
</body>
</html>

What's the best way to guide an engineer to make an IOT accessory?

Here are some ideas:
1. Raspberry pi and Arduino might have good documentations
2. In a general sense, the guidance to make an IOT accessory could borrow from the best practices to guide someone build a hardware accessory. For example, making a bluetooth speaker / headphone.

This is the starting place: https://staceyoniot.com/podcast-how-to-build-your-own-iot-device/