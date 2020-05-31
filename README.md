# YARD
YARD is a visual playlist concept design to capture elements from my backyard. I designed it to share the experience of being outside during quarantine. 
Javascript animation: Copyright © 1986 - ∞, Blotter / Bradley Griffith / http://bradley.computer 

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>YARD</title>
    <script src="https://cdn.rawgit.com/bradley/Blotter/master/build/blotter.min.js"></script>
    <script src="https://rawgit.com/bradley/Blotter/master/build/materials/liquidDistortMaterial.js"></script>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div id="main"></div>

    <audio controls loop>
        <source src="YARD Playlist.mp3" type="audio/mp3">
      Your browser does not support the audio element.
      </audio>

    <h1>
        FRANK OCEAN.....................At Your Best (cover)<br>
        ORION SUN.......................Coffee For Dinner<br>
        SUNNI COLON.....................Baby I Don't Mind<br>
        KARI FAUX.......................Color Theory<br>
        HALL & OATES....................I Can't Go For That (Instrumental)<br>
        MARVIN GAYE.....................I Want You<br>
        ORION SUN.......................Mango (Freestyle)<br>
        NICK HAKIM......................Needy Bees<br>

 </h1>
 

 <h2>
   I do not own the rights to this music.
 </h2>


<!-- Copyright © 1986 - ∞, Blotter / Bradley Griffith / http://bradley.computer -->

<script>

    container = document.getElementById("main");

    const text = new Blotter.Text("YARD", {
        family: "serif",
        size: 350,
        fill: "#ffd700"
    });

    let material = new Blotter.LiquidDistortMaterial();

    material.uniforms.uSpeed.value = 0.1;
    material.uniforms.uVolatility.value = 0.1;
    material.uniforms.uSeed.value = 0.1;

    let blotter = new Blotter(material, {
        texts: text
    });

    let scope = blotter.forText(text);

    scope.appendTo(container);

</script>


</body>
</html>
