# Welcome

<!-- Her kan du skrive tekst som kommer i toppen af siden -->


<!-- Niks pille, med mindre du ved hvad du gør! -->
<div id="imageshere" />
<script>
  var url = "https://raw.githubusercontent.com/tofteapp/imageapp/master/";
  var exts = ["jpg", "JPG", "jpeg", "JPEG", "png", "PNG", "gif"];
  var imageNotFound = function () {
    this.hidden = true;
  }
  
  for (var i=1; i<=10; i++) {
    for (var j=0; j<exts.length; j++) {
      var img = new Image();
      img.addEventListener('error', imageNotFound);
      img.src = url + i + "." + exts[j];
      document.getElementById("imageshere").appendChild(img);
      document.getElementById("imageshere").appendChild(document.createElement("BR"));
    }
  }
  
  // remove head and footer:
  document.getElementsByClassName("page-header")[0].hidden = true;
  document.getElementsByClassName("site-footer")[0].hidden = true;
</script>


<!-- Her kan du skrive tekst som kommer i bunden af siden -->
