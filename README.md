<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Breathe</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css"
        integrity="sha384-9aIt2nRpC12Uk9gS9baDl411NQApFmC26EwAOH8WgZl5MYYxFfc+NcPb1dKGj7Sk" crossorigin="anonymous">
    <link rel="stylesheet" href="breathe.css">
    <link href="https://fonts.googleapis.com/css2?family=Raleway:wght@800&amp;display=swap" rel="stylesheet">  
</head>
<body>
    <div id="container" class="body container-sm">
        <!-- <h1 id="header" >Testing 1,2,3</h1> -->
        <div id="headings" class="">
            <h1 id="breathaction" class="display-3 text-primary text-center">/Breathe/</h1>
            <h2 id="count" class="display-4 text-warning text-center"></h1>
        </div>
        <form id='actions' action="" onsubmit="return false"> <!--Prevents the form from resetting!!!-->
            <div class="col-sm text-center">
                <div class="text-info">Choose a breathing exercise</div>

                <div class="py-2">
                    <!-- <label for="select" id="presets">Choose from our presets</label> -->
                    <select name="select" id="presets" class="action mb-3">
                        <option value="none" class="text-success">----Custom----</option>
                        <option value="boxFour" selected="selected">Box Breathing (4-4-4-4)</option>
                        <option value="boxSix">Box Breathing (6-6-6-6)</option>
                        <option value="fourSevenEight">4-7-8</option>
                        <option value="fourTwoEight">4-2-8</option>
                        <option value="resonantFive">Resonant (5-5)</option>
                    </select>

                    <p  id="presets" class="text-info pt-2">Or, enter a custom one!</p>
                </div>
                <section id="customization">
                    <div class="pb-2">
                        <!-- <label for="select">Choose an action</label> -->
                        <select name="select" id="action1" class="action">
                            <option value="Inhale" selected="selected">Inhale</option>
                            <option value="Exhale">Exhale</option>
                            <option value="Hold">Hold</option>
                        </select>
                        for
                        <input  class="customslider" type="range" id="act1duration" name="act1duration" max="15" min="2" value="4">
                        <output class="act1text"></output> seconds
                    </div>

                    <div class="py-2">
                        <!-- <label for="select">Choose an action</label> -->
                        <select name="select" id="action2" class="action">
                            <option value="Inhale">Inhale</option>
                            <option value="Exhale" >Exhale</option>
                            <option value="Hold" selected="selected">Hold</option>
                        </select>
                        for
                        <input class="customslider" type="range" id="act2duration" name="act2duration" max="15" min="2" value="4" >
                        <output class="act2text"></output> seconds
                    </div>

                    <div class="py-2">
                        <!-- <label for="select">Choose an action</label> -->
                        <select name="select" id="action3" class="action">
                            <option value="Inhale">Inhale</option>
                            <option value="Exhale" selected="selected">Exhale</option>
                            <option value="Hold">Hold</option>
                            <option value="None">None</option>
                        </select>
                        for
                        <input class="customslider" type="range" id="act3duration" name="act3duration" max="15" min="2" value="4">
                        <output class="act3text"></output> seconds
                    </div>
                    <div class="py-2">
                        <!-- <label for="select">Choose an action</label> -->
                        <select name="select" id="action4" class="action">
                            <option value="Inhale">Inhale</option>
                            <option value="Exhale">Exhale</option>
                            <option value="Hold" selected="selected">Hold</option>
                            <option value="None" >None</option>
                        </select>
                        for
                        <input class="customslider" type="range" id="act4duration" name="act4duration" max="15" min="2" value="4">
                        <output class="act4text"></output> seconds
                    </div>
                </section>

                <div class="py-3">
                    <label for="numcycles">Number of cycles:</label>
                    <input type="range"  id="numcycles" name="numcycles" max="50" min="1" value="8">
                    <output class="numcyclestext"></output> <el id="numcyclestext">cycles</el>   
                </div>

                <button id="breathebutton" class="btn btn-primary" >Start</button>
                
            </div>
        </form>
        <div class="d-flex justify-content-center">
            <button id="stop" class="btn btn-secondary">Stop</button>
        </div>   
</div>
<script src="breathe.js"></script>
</body>
</html>
