# Triple-A
Our website is a place that started in an instant. We had discussed making a website together before, but we had never actually done it. When this project was mentioned, however, we knew that we should jump at the opportunity to work together. Although at times we disagree, we work together grandly.

-Make sure to hover over the word cloud on the home page, and notice the design.

-Please hover over our portfolio, and see how each picture links to a special spot on another page. 


-PHP Submit Button:

	<form action="send.php" class="form">
      <label class="label">First name:</label>
      <input name="firstname" id="firstname" type="text" ><br>
      <label class="label">Last name:</label><br> 
      <input name="lastname"  id="lastname" type="text"><br>
      <label class="label">Date of Birth:</label><br>
      <input name="dob" id="dob" type="text" ><br>
      <label class="label">Phone Number:</label><br> 
      <input name="number" id="number" type="text" ><br>
      <label class="label">Current Work Place:</label><br> 
      <input name="cwp" id="cwp" type="text" ><br>
      <label class="label">Address:</label><br> 
      <input name="address" id="address" type="text" ><br><br>
      <label class="label">Anything else you wish to tell me?</label><br>
      <textarea name="comments" id="comments"></textarea>
      <input name="submit" type="submit" value="Send" />
	</form>

	<?php 

	$firstname=$_POST['firstname'];
	$lastname=$_POST['lastname'];
	$dob=$_POST['dob'];
	$number=$_POST['number'];
	$cwp=$_POST['cwp'];
	$address=$_POST['address'];
	$comments=$_POST['comments'];

	$date=gmdate("M d Y");


	print"<p><b>$date</b></p>";
	print"<p>Thank you $firstname $lastname! We will get back to you.</p>";


	$to="aleya.adams@students.jmcss.org";

	$subject="Application";

	$body="Date:$date \n Subject:$subject \n First Name:$firstname \n Last Name:$lastname \n Date of Birth:$dob \n Phone Number:$number \n Current Work 		Place:$cwp \n Addresss:$address \n Additional Information:$comments \n\n";

	mail($to,$subject,$body);

	?>



	We would have done this using PHP, but since we knew it would not work once it was downloaded, we chose to make it link to another page instead. The 		button does not actually send the file to email.

-Check out the different fonts we used.

-the pricing table is organized the way it is because we believe if a client is on a budget they can easily see what they need and the price. This will lead  to a more productive site in the end.

-We have a logo icon on the tab of the web browser, which works on Firefox and Internet Explorer, but sometimes does not work on Google Chrome (a problem many people have ran into). Even though it does not show up on the tab, it does not affect the website significantly.

-On the apply confirmation page, we chose to write the confirmation in Old English and have a Mars landing animation to show old and new coming together to a beautiful combination of websites.
