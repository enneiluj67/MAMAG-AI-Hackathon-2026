<!DOCTYPE html>
<html>
	<head>
		<!-- Title -->
		<title> Project MAMAG: Monitoring and Management of Academic Goals </title>
		
		<!-- Meta Tags -->
		<meta charset="UTF-8">
		<meta name="author" content="CAMP MAMAG">
		<meta name="description" content="An AI-Based PISAY Student Clearance Monitoring System">
		<meta name="revised" content="02/02/2026">
		
		<style>
			/* CSS Design for Body, Background, Text */
			body {background-color: #d1f3ff; font-family: Arial; text-align: center; padding: 50px;}
			body {background-image: url('pisay-cbzrc.jpg'); background-size: cover; background-repeat: no-repeat; background-position: center;}
			header {background-color: #79bcd5; font-size: 18px; padding: 4px; border-radius: 30px;}
			h1 {color: #2c3e50; margin-bottom: 20px;}
			body::before {content: ""; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background-color: rgba(0, 0, 0, 0.5); z-index: -1;}
			
			/* CSS Design for Input and Login */
			input {font-size: 20px; width: 400px; height: 30px;}
			.login-container { background-color: rgba(255, 255, 255, 0.85); margin-top: 20px; padding: 40px; border-radius: 12px; box-shadow: 0 8px 20px rgba(0,0,0,0.2); display: inline-block;}
			button.login {background-color: #43a047; color: white; padding: 10px 20px; border: none; border-radius: 6px; font-size: 16px; cursor: pointer;}
			button.login:hover {background-color: #66bb6a;}
		</style>
	</head>
	<body>
		<!-- Header -->
		<header>
			<h2> Philippine Science High School <br>
			CALABARZON Region Campus in Batangas City </h2>
			<h2> Year-End Clearance, S.Y. 2025 - 2026 </h2>
		</header>
		
		<!-- Login -->
		<div class="login-container">
			<h1> Login Page </h1>
			<input type="email" id="email" placeholder="Email"><br><br>
			<input type="password" id="password" placeholder="Password"><br><br>
			<button class="login" onclick="login()"> Login </button>
		</div>
		
		<!-- Login Function -->
		<script>
			function login() {
				const email = document.getElementById("email").value;
				const password = document.getElementById("password").value;

				if (email === "gurongbayan@cbzrc.pshs.edu.ph" && password === "sixseven") {
					window.location.href = "page2_teacher.html";}
				else if (email === "iskolarngbayan@cbzrc.pshs.edu.ph" && password === "sixseven") {
					window.location.href = "page3_student.html";}
				else {
					alert("Invalid email or password");}
			}
		</script>
	</body>
</html>
