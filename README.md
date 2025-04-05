# Patient-OPD-
<html>
    <head>
        <title>Patient Informtion</title>
        <link rel="icon" type="image/x-icon" href="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQj-mq5EBi3wf0XA8Kt_Bae6JXpxlSqBTWsww&s">
        <style>
            .datetime {
                position: fixed;
                top: 10px;
                right: 10px;
                font-size: 20px;
            }
            .container{
            background:skyblue;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            max-width: 400px;
            margin: auto;
            }
            input {
            width: 80%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
            }
        button {
            padding: 10px 20px;
            background-color: #28a745;
            color: blue;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #218838;
        }
        .H1{
            text-align:"center";
        }
        </style>   
 </head>
    <body>
    <H1 >Welcome</H1>
    <div class="datetime" id="currentDateTime"></div>
<script>
        function updateDateTime() {
            let now = new Date();
            let formattedDateTime = now.toLocaleString();
            document.getElementById("currentDateTime").textContent = formattedDateTime;
        }
        setInterval(updateDateTime, 1000);
        updateDateTime();
    </script>
  <div class="container"> 
        <h3>Enter Patient's Details: </h3>
        Patient Name:
        <input type="text" id="name" placeholder="First Name"> 
        <input type="text" id="name" placeholder="Last Name"><br><br>
        Patient Age:
        <input type="number" id="Age" placeholder="Age">
        <br> <br>
        Patient Blood Pressure:
        <input type="text" id="name" placeholder="BP"><br> <br>
        Patient SPO<sub>2</sub>:
        <input type="number" id="pulse" placeholder="Oxymeter"><br> <br>
        Patient Complications:
        <textarea name="Patient Complications" rows="5" cols="30" placeholder="patient Complications"></textarea>
        <br> <br>
        Choose Doctor:  
        <select>
        <option>Dr.Rama Krishna</option>
        <option>Dr.Sathya</option>
        <option>Dr.Ramya </option>
        <option>Dr.Arjun</option>
    </select>
    <br>
    <br>
    
   
</div>

   </body>
</html>
