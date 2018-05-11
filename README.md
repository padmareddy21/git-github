# git-github
<html>
<body>
<form name="f1" action="log.php" method="post" enctype="multipart/form-data" onsubmit="return check()">
<script language="javascript">
function check()
{
 if(document.f1.name.value=="")
  {
    document.getElementById("n").innerHTML="*enter your name";
	document.f1.name.focus();
	return false;
  }
  else
  {
   document.getElementById("n").innerHTML="";
  }
 if(document.f1.fn.value=="")
  {
     document.getElementById("n1").innerHTML="Please Enter fathers name";
	document.f1.fn.focus();
	return false;
  }
  else
  {
   document.getElementById("n1").innerHTML="";
  }
  if(document.f1.emailid.value=="")
  {
     document.getElementById("n2").innerHTML="Please Enter your Email Address";
	document.f1.emailid.focus();
	return false;
  }
  else
  {
  e=document.f1.emailid.value;
		f1=e.indexOf('@');
		f2=e.indexOf('@',f1+1);
		e1=e.indexOf('.',f1+1);
		e2=e.indexOf('.',e1+1);
		n=e.length;
		if(!(f1>0 && f2==-1 && e1>0 && e2==-1 && f1!=e1+1 && e1!=f1+1 && f1!=n-1 && e1!=n-1))
		{
			document.getElementById("n2").innerHTML="Please Enter your Email Address";
			document.f1.emailid.focus();
			return false;
		}
		 else
  {
   document.getElementById("n2").innerHTML="";
  }
	}
 
 if(document.f1.pwd.value=="")
  {
    document.getElementById("n3").innerHTML="Please Enter Your Password";
	document.f1.pwd.focus();
	return false;
  } 
  else
  {
   document.getElementById("n3").innerHTML="";
  }
    if(document.f1.mobileno.value=="")
	{
      document.getElementById("n4").innerHTML="This is not a valid phone number";
	  document.f1.mobileno.focus();
      return false;
  }
   return true;
  }
if(document.f1.photo.value=="")
 {
     document.getElementById("n5").innerHTML="should upload";
     document.f1.photo.focus();
 }
 else
  {
     
</script>
<table  bgcolor="black" align="center" >
<tr>
<td colspan=2>
<center><h1><font color="white"> Registration Form</h1></center>
</td>
</tr>
<tr>
<td><font color="yellow">Name</font></td>
<td><input type="text" name="name" onblur="check()"><font color="red" id="n"></font></td>
</tr> 
<tr> <td><font color="yellow">Father Name</td>
<td><input type="text" name="fn" onblur="check()"><font color="red" id="n1"></font></td>
</tr>
<tr>
<td><font color="yellow">DOB</td>
<td><input type="text"  size="30"></td>
</tr>
<tr>
<td><font color="yellow">Sex</td>
<td><input type="radio" name="sex" value="male" size="10"><font color="white">Male
<input type="radio" name="sex" value="Female" size="10"><font color="white">Female</td>
</tr>
<tr>
<td><font color="yellow">EmailId</td>
<td><input type="text" name="emailid" id="emailid" size="30" onblur="check()"><font color="red" id="n2"></font></td>
</tr> 
<tr>
<td><font color="yellow">password</td>
<td><input type="text" name="pwd" onblur="check()"><font color="red" id="n3"></font></td>
</tr> 
<tr> <td><font color="yellow">Course</td>
<td><select name="Course">
<option value="-1" selected>select..</option>
<option value="B.Tech">B.TECH</option>
<option value="polytechnic">polytechnic</option>
<option value="mba">mba</option>
</select></td>
</tr>
<tr>
<td><font color="yellow">Permanent Address</td>
<td><input type="text" name="paddress" id="paddress" size="30"></td>
</tr>
<tr>
<td><font color="yellow">City</td>
<td>
 <input list="browsers" name="browser">
  <datalist id="browsers">
<option value="New Delhi">NEW DELHI</option>
<option value="Mumbai">MUMBAI</option>
<option value="khammam">khammam</option>
<option value="vijayavada">vijayawada</option>
<option value="sathupally">sathupally</option>
</select></td>
</tr>
<tr>
<td><font color="yellow">District</td>
<td><select name="District">
<option value="-1" selected>select..</option>
<option value="khammam">khammam</option>
<option value="krishna">krishna</option>
<option value="warangal">warangal</option>
</select></td>
</tr>
<tr>
<td><font color="yellow">State</td>
<td><select Name="State">
<option value="-1" selected>select..</option>
<option value="telangana">telangana</option>
<option value="andra pradesh">andra pradesh</option>
<option value="mumbai">mumbai</option>
<option value="new delhi">new delhi</option>
<option value="Rajasthan">Rajasthan</option>
</select></td>
</tr>
<tr>
<td><font color="yellow">PinCode</td>
<td><input type="text" name="pincode" id="pincode" size="30"></td>
</tr>
<tr>
<td><font color="yellow">MobileNo</td>
<td><input type="text" name="mobileno" id="mobileno" size="30" onblur="check()"><font color="red" id="n4"></font></td>
</tr>
</tr>
<tr>
<td><font color="yellow">photo</td>
<td><input type="file" name="f1"></td>
</tr>
<tr>
<td><font color="yellow">skills</td>
<td><input type="checkbox" name="c[]" value="c">C</td>
<td><input type="checkbox" name="c[]" value="c++">C++</td>
<td><input type="checkbox" name="c[]" value="java">JAVA</td>
</tr>

<tr >
<td align="center" colspan=2><input type="reset" value="Reset">
<input type="submit" value="Submit Form"></td>
</tr>
</table>
</form>
</body>
</html> 
