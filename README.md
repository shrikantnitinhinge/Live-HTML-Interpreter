<html>
<head>
    <title>Live HTML Interpreter</title>

    <script src="https://kit.fontawesome.com/7e49c991d7.js" crossorigin="anonymous"></script>

    <script>
    function show_output()
    {
    document.getElementById("output").innerHTML =   document.getElementById("textArea").value;
    }
    </script>

    <style>
    body{
        background-color: #A5362D;
        background-image: linear-gradient(to right, #2D41A5, #904e95);  
        font-family: Verdana,    sans-serif;   
    }   
    
    h1{
        text-align: center;
        color: white;
        text-shadow: 1px 1px 1px #ffeead, 1px 1px 1px # ffeead, 1px 1px 1px #ffeead; 
        font-family: Georgia, serif;    
    }   
    
    div{
        float: left;
        width: 50%;
        padding: 10px;
        height: 100%;
        border-radius: 25px;
    }
    
    * {
      box-sizing: border-box;
    }
    
    #input{
        background-color: #A52D41 ;
        /*border: 5px solid black;
        border-radius: 5px;*/
    }
    
    #textArea{
        display: block;
        overflow-x: hidden; 
        overflow-y: scroll;
        width: 100%;
        height: 90%;
        padding: 10px;
    }
    
    #output{
        background-color:#2DA5A5 ;
        /*border: 5px solid black;
        border-radius: 5px;*/
    }
    </style>
</head>
<body>

<h1> <i class="fab fa-html5"></i> Live HTML Interpreter </h1>

<div id="input">
    <p>  Enter your HTML code here:</p>
    <textarea id="textArea"
    onkeyup="show_output()">
    </textarea>
</div>

<div id="output">
    <p> Output will appear here. </p>
</div>

</body>
</html>
