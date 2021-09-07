<?php
	if(isset($_POST['name'])) 
	{
		$output= array();
		$name= ($_POST["name"] !='') ? $_POST['name'] : '';
		$goal1=($_POST["goal1"] !='') ? $_POST['goal1'] : '';
		$goal2=($_POST["goal2"] !='') ? $_POST['goal2'] : '';
		$goal3=($_POST["goal3"] !='') ? $_POST['goal3'] : '';
		if ($goal1 !='' && $goal2 !='' && $goal3 !='') {

			$message=$goal1.", ".$goal2.", ".$goal3;
			$dataFile='data.log';
			file_put_contents($dataFile, "");
			if (file_exists($dataFile)) {
				$fh = fopen($dataFile, 'a');
				fwrite($fh, $message."\n");
			} else {
				$fh = fopen($dataFile, 'w');
				fwrite($fh, $message."\n");
			}
			fclose($fh);
			$output['status']="success";
			$output['message']="Thanks for your answers.";
		}
		else{
			$output['status']="missing_parameter";
			$output['message']="Please fill in all the fields.";
		}
		echo json_encode($output);
		exit;
	}
?>
	<!DOCTYPE html>
	<html>
	<head>
	<title>Survey Form</title>
	<link href="https://fonts.googleapis.com/css?family=Roboto" rel="stylesheet"> 
	<style type="text/css">
	body{
			font-family: 'Roboto', sans-serif;
		}
	.error{
		color:red;
	}
	.success{
		color:green;
	}
	.overlay{
		display: none;
	}
	.form_block{
		min-width: 300px;
		height: 400px;
		background-color: #fff;
		position: absolute;
		left: 0;
		right: 0;
		top: 0;
		bottom: 0;
		margin: auto;
		max-width: 75%;
		overflow: auto;
		text-align: center;
	}
	.field_label {
		font-size: 18px;
		font-weight: 600;
		color: #000;
	}
	p {

		width: 100%;
		padding: 18px 0px;

	}
	p input {

		width: 40%;
		margin-left: 27px;
		height: 30px;
		border: 1px solid #e2e2e2;
			font-size: 16px;
		color: #141212;
		padding-left: 10px;
	}
	.field_label {

		font-size: 18px;
		font-weight: 600;
		color: #000;
		width: 40%;

	}
	h3 {

		font-size: 24px;
		font-weight: bold;

	}
	#submit_survey {

	background-color: #5885C4;
	border: 0px;
	padding: 10px 20px;
	border-radius: 3px;
	color: #fff;
	font-weight: 500;
	font-size: 16px;

	}
	.goal_div p {

		padding: 2px 0px;

	}
	/* The Modal (background) */
	.modal {

		display: none; /* Hidden by default */
		position: fixed; /* Stay in place */
		z-index: 1; /* Sit on top */
		padding-top: 100px; /* Location of the box */
		left: 0;
		top: 0;
		width: 100%; /* Full width */
		height: 100%; /* Full height */
		overflow: auto; /* Enable scroll if needed */
		background-color: rgb(0,0,0); /* Fallback color */
		background-color: rgba(0,0,0,0.4); /* Black w/ opacity */

	}

	/* Modal Content */
	.modal-content {

		background-color: #fefefe;
		margin: auto;
		padding: 20px;
		border: 1px solid #888;
			width: 33%;
		border-radius: 6px;

	}

	/* The Close Button */
	.close {

		color: #aaaaaa;
		float: right;
		font-size: 28px;
		font-weight: bold;
		top: -15px;
		position: relative;
		right: -5px;

	}

	.close:hover,
	.close:focus {

		color: #000;
		text-decoration: none;
		cursor: pointer;

	}
	#user_name {

	    padding-right: 0px;
	    width: 40%;
	    margin-left: 4px;

	}
	.field_label.name_label {
	    left: -23px;
	    position: relative;
	}
	@media only screen and (min-width: 320px) and (max-width: 500px)
	{
		.field_label{
			display: none;
		}
		p input {

			width: 80%;
			margin: 0px 0px;
		}
		#user_name {

		    padding-right: 0px;
			width: 80%;
			margin-left: 0px;

		}

	}
</style>
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.4/jquery.min.js"></script>
	<script type="text/javascript">
	$(document).ready(function(){
		$('#submit_survey').on('click', function(){
			$('.message').remove();
			var name=$('#user_name').val();
			var goal1=$('#goal1').val();
			var goal2=$('#goal2').val();
			var goal3=$('#goal3').val();
			$.ajax({
				dataType: 'json', 
				data: {
				name:name, 
				goal1:goal1, 						
				goal2:goal2,
				goal3:goal3
			},
				type: 'post',
				success: function (response) {
					var message= '<span class="message">'+response.message+'</span>';
					if (response.status == 'success') {	

						$('#myModal p').html(message);
						$('#myModal p').addClass('success');
						$('#myModal').show();

					}
					else if(response.status == 'missing_parameter'){
						$('#myModal p').html(message);
						$('#myModal p').addClass('error');
						$('#myModal').show();
					}
				},
				error: function (response) {

				}
			});
		})

			$('.close').on('click', function(){
				$('#myModal').hide();
			})

	})
	</script>
	</head>
	<body>
	<div class="full_block">
	<!-- Form div section  -->
	<div class="form_block">
	<form action="" method="post" id="survey_form">
	<p> <label class="field_label name_label">Your name:</label> <input id="user_name" type="text" placeholder="Please leave your name here" name="user_name"></p>
		<h3>What are your 3 major life goals?</h3>
		<div class="goal_div">
		<p> <label class="field_label">Goal #1:</label> <input id="goal1" type="text" placeholder="Put your goal #1 here" name="user_name"></p>
		<p> <label class="field_label">Goal #2:</label> <input id="goal2" type="text" placeholder="Put your goal #2 here" name="user_name"></p>
		<p> <label class="field_label">Goal #3:</label> <input id="goal3" type="text" placeholder="Put your goal #3 here" name="user_name"></p>
		</div>
		<div class="submit_section">
		<input id="submit_survey" name="survey_submit" type="button" value="Submit">		 
		</div>
		</form>		
		</div>
		</div>
		<div id="myModal" class="modal">
		<!-- Modal content -->
		<div class="modal-content">
		<span class="close">&times;</span>
			<p>Some text in the Modal..</p>
			</div>

			</div>
			</body>
			</html>

