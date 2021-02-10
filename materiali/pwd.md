---
layout: page
title: "Materiali didattici"
category: "materiali didattici"
permalink: "/materiali/"
image: "http://www.concertoconmammaepapa.it/web/wp-content/uploads/2019/08/musica-nova-14-dicembre-2019.jpg"
card:
  image: "/image/monserrat_canta.jpg"
  title: " Monserrat Olavarria"
  subtitle: "cantante <br> docente di musica"
  text: "Mi dedico alla composizione di materiale originale, canzoni, canti e filastrocche che utilizzo nei propri percorsi didattici con i bambini di diverse età."
  link: "/chisono/"
social:
  youtube: "https://www.youtube.com/channel/UCMQJkzvobU3ZikrzYaY3x7w/featured/"
  me: "https://m.me/avenidamerica/"
  facebook: "https://www.facebook.com/avenidamerica/"
sidebar:
  image: "/image/tiritinlalla_1980.jpg"
  title: ""
  subtitle: "Tiritinlallà"
  text: "il mio ultimo disco"
  link: "/dischi/tiritinlalla/"
---


	<div id="loginbox" class="lightbox" >
		<div class="horizontal">
			<div class="vertical">
				<div class="box">
					<input style="margin: 16px; text-align: center;" id="password" type="password" placeholder="password" /> <br />
					<button id="loginbutton" type="button">Enter</button>
					<p id="wrongPassword" style="display: none">wrong password</p>
				</div>
			</div>
		</div>
	</div>




	<script type="text/javascript" src="https://code.jquery.com/jquery-1.12.0.min.js"></script>


	 <script type="text/javascript" src="https://rawcdn.githack.com/chrisveness/crypto/7067ee62f18c76dd4a9d372a00e647205460b62b/sha1.js"></script>

	<script type="text/javascript">
	"use strict";


	function loadPage(pwd) {

		var hash= pwd;
		hash= Sha1.hash(pwd);
		var url= hash + "/index.html";

		$.ajax({
			url : url,
			dataType : "html",
			success : function(data) {

				window.location= url;

			},
			error : function(xhr, ajaxOptions, thrownError) {


				parent.location.hash= hash;

				//$("#wrongPassword").show();
				$("#password").attr("placeholder","wrong password");
				$("#password").val("");
			}
		});
	}


	$("#loginbutton").on("click", function() {
		loadPage($("#password").val());
	});
	$("#password").keypress(function(e) {
		if (e.which == 13) {

			loadPage($("#password").val());
		}
	});
	$("#password").focus();

	</script>