<!Doctype html>
<html>
<title>Assignment</title>
<style>
	    fieldset{       
                  background-color:dodgerblue;
                  padding-top: 75px;
                  padding-right: 100px;
                  padding-bottom: 50px;
                  padding-left: 100px;
		        }
		h1{
			 font-size:30px;
		     text-align: center;
		     background-color:cyan;
		  }  
		body{
			      padding-top: 100px;
                  padding-right: 200px;
                  padding-bottom: 50px;
                  padding-left: 200px;
		    }
</style>
<fieldset>
<head>
	<script type='text/JavaScript'>
		function validationform(){
			var x=document.myform.name.value;

			var y=document.myform.lname.value;

			if((x ==null ) && (y == null)){
				alert("Missing First Name or Last Name");
				return false;
			}
			else
			{
				return true;
			}
			var m=document.myform.email.value;
			if(m.indexof('@')<=0)
			{
				document.getElementById("Messege").innerHTML="Enter Valid email";
				return false;
			}
			if(m.charAt(m.length-4)!='.') && (m.charAt(m.length-3)!='.')
			{
				document.getElementById("Messege").innerHTML="Enter Valid email";
				return false;
			}

	</script>
</head>
<body bgcolor="cyan">
		<h1>Sharedrop Registration </h1>
		
		<form name="myform" onsubmit="return validationform()" >
		First Name:<input type="text" name="fname" placeholder="e.g Jhon"  /><br><br>

		Last Name:<input type="text" name="lname" placeholder="e.g Disuza"></input> <br><br>

        Email     :<input type="text" name="email"placeholder="e.g Jhon@gmail.com" value="" size="30"></input>
        <span id="Messege"> </span><br><br>

        Birth Date:<input type="Birth" name="dob"   placeholder=" dd/mm/yy" size="">
        <br><br>

        Phone Number:<input type="Phone" name="inputno" placeholder="e.g +91" size="12"><br><br>

        Password     :<input type="pass" name="Password" size="20"  ><br><br>

         
 		<input type="submit" value="Register" >
		</form>
</body>
</fieldset>
</html>
