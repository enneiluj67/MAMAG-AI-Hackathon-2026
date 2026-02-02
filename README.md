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
		
		<script>
			<!-- Approve Function -->
			function approve(button) {
				const row = button.parentElement.parentElement;
				row.cells[2].textContent = "None";
				row.classList.add("approved");
				button.disabled = true;
				button.innerText = "Approved";
			}
			<!-- Search Student -->
			function searchStudent() {
				const input = document.getElementById("search").value.toLowerCase();
				const rows = document.querySelectorAll("table tr");

				for (let i = 1; i < rows.length; i++) {
					const name = rows[i].cells[1].textContent.toLowerCase();
					rows[i].style.display = name.includes(input) ? "" : "none";
				}
			}
		</script>

		<style>
			/* CSS Design for Body and Text */
			body {background-color: #d1f3ff; font-family: Arial; text-align: center; padding: 50px;}
			body {background-image: url('pisay-cbzrc.jpg'); background-size: cover; background-repeat: no-repeat; background-position: center;}
			header {background-color: #79bcd5; font-size: 18px; padding: 4px; border-radius: 30px;}
			body::before {content: ""; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background-color: rgba(0, 0, 0, 0.5); z-index: -1;}
			h1 {color: white; margin-bottom: 10px; font-size: 32px;}
			h3 {margin-bottom: 5px; font-weight: 600;}
			h4 {margin-top: 0; font-weight: normal;}
			.info {color: white;}
			
			/* CSS Design for Approve Button */
			button {background-color: #43a047; color: white; padding: 8px 14px; border-radius: 6px; border: none; font-weight: 600; cursor: pointer;}
			button:hover {background-color: #88f575;}
			button:disabled {background-color: #aaa; cursor: not-allowed;}

			/* CSS Design for Data Table */
			table {width: 100%; border-collapse: collapse; background-color: white; border-radius: 10px; overflow: hidden; box-shadow: 0 4px 12px rgba(0,0,0,0.08); margin: 20px auto 30px;}
			th, td {padding: 12px 16px; border: 2px solid #e0e0e0;;}
			th {background-color: #2c3e50; color: white;}
			tr:hover {background-color: #eef3ff;}
			.approved td {background-color: #88f575;}
			
			/* CSS Design for Search Bar */
			#search {width: 400px; padding: 8px; margin: 10px auto; border-radius: 6px; border: 1px solid #ccc; font-size: 16px;
}
		</style>
	</head>
	<body>
		<h1> Teacher Dashboard </h1>
		
		<!-- Teacher Information -->
		<div class = "info">
			<h3> Ms. Math E. Matics </h3>
			<h4> Special Science Teacher II </h4>
			<p> <strong> Class: </strong> 7 - Emerald (Mathematics 1) </p>
		</div>
		
		<!-- Data Table -->
		<input type="text" id="search" placeholder="Search student name..." onkeyup="searchStudent()">
		<table>
			<tr>
				<th> Grade and Section </th>
				<th> Name of Student </th>
				<th> Missing Requirements </th>
				<th> Approve </th>
			</tr>
			<tr>
				<td> 7 - Emerald </td>
				<td> Bunagan, Beethoven "Michael V" Del Valle </td>
				<td> AA2: Problem Set on LEOV </td>
				<td> <button onclick="approve(this)"> Approve </button> </td>
			</tr>
			<tr>
				<td> 7 - Emerald </td>
				<td> Cermeño, Cipriano "Redford White" II </td>
				<td> None </td>
				<td> <button onclick="approve(this)"> Approve </button> </td>
			</tr>
			<tr>
				<td> 7 - Emerald </td>
				<td> De Leon, Jose Maria "Joey" Ramos </td>
				<td> None </td>
				<td> <button onclick="approve(this)"> Approve </button> </td>
			</tr>
			<tr>
				<td> 7 - Emerald </td>
				<td> Delas Alas, Martina Eileen "Ai-Ai" Hernandez </td>
				<td> AA1: Creative Output </td>
				<td> <button onclick="approve(this)"> Approve </button> </td>
			</tr>
			<tr>
				<td> 7 - Emerald </td>
				<td> Gonzaga, Catherine "Alex" Cruz </td>
				<td> None </td>
				<td> <button onclick="approve(this)"> Approve </button> </td>
			</tr>
			<tr>
				<td> 7 - Emerald </td>
				<td> Quizon, Rodolfo "Dolphy" Vera </td>
				<td> AA1: Creative Output </td>
				<td> <button onclick="approve(this)"> Approve </button> </td>
			</tr>
			<tr>
				<td> 7 - Emerald </td>
				<td> Requiestas, Renato "Rene" Licup </td>
				<td> None </td>
				<td> <button onclick="approve(this)"> Approve </button> </td>
			</tr>
			<tr>
				<td> 7 - Emerald </td>
				<td> Revillame, Wilfredo "Willie" Buendia </td>
				<td> AA1: Creative Output </td>
				<td> <button onclick="approve(this)"> Approve </button> </td>
			</tr>
			<tr>
				<td> 7 - Emerald </td>
				<td> Sotto, Marvic Valentin "Vic" Castelo </td>
				<td> FA6: Graphing </td>
				<td> <button onclick="approve(this)"> Approve </button> </td>
			</tr>
			<tr>
				<td> 7 - Emerald </td>
				<td> Viceral, Jose Marie "Vice Ganda" Borja </td>
				<td> None </td>
				<td> <button onclick="approve(this)"> Approve </button> </td>
			</tr>
		</table>
	</body>
</html>
