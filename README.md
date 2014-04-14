<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=windows-1251"/>
 <link rel="stylesheet" media="screen,projection,tv" href="//support.cdn.mozilla.net/static/css/common-min.css?build=f7d846f" />
<title>Форма</title>
</head>
<body>
<script type="text/javascript">
function poschitat(){
var fytbolku_club_tovara=1;
if (document.forms[0].fytbolku_club[0].checked==true)
 {
 fytbolku_club_tovara=0;
 price=250;
 }
if (document.forms[0].fytbolku_club[1].checked==true)
{
fytbolku_club_tovara=1;
price=270;
}
if (document.forms[0].fytbolku_club[2].checked==true)
{
fytbolku_club_tovara=2;
price=350;
}
if (document.forms[0].fytbolku_club[3].checked==true)
{
fytbolku_club_tovara=3;
price=600;
}
if (document.forms[0].fytbolku_club[4].checked==true)
{
fytbolku_club_tovara=4;
price=365;
}
if (document.forms[0].fytbolku_club[5].checked==true)
{
fytbolku_club_tovara=5;
price=1000;
}

var text="Ціна замовлення="+price;
var price = document.body.getElementsByClassName("price")[0];
price.innerHTML=text;
}
</script>
<p>
<form method="GET" action="login.php" enctype="multipart/form-data" name="login">

<form id="contact-form" action="login.php" method="post"> 
	            <label for="login">login:</label>
	            <input type="text" login="login" id="login" value="" />
<p></p>
	            <label for="password">password:</label>
	            <input type="text" login="password" id="password" value="" />
<p></p>
	            <font size = "14" color="blue"> <center>Футболку якого Футбольного Клубу ви обираєте?</font></center>
<p></p>

		<input type="radio" name="fytbolku_club" value="Barsa"><b>Barselona</b>
<p></p>
	            <input type="radio" name="fytbolku_club" value="Milan"><b>Milan</b>
<p></p>
	            <input type="radio" name="fytbolku_club" value="Inter"><b>Inter</b>

<p></p>
<input type="radio" name="fytbolku_club" value="Real"><b>Real</b>

<p></p>
<input type="radio" name="fytbolku_club" value="PSG"><b>PSG</b>

<p></p>
<input type="radio" name="fytbolku_club" value="Atletico"><b>Atletico</b>

<p></p>

<B>Кількість</B> <input type="text" name="login" size="10"maxlength="20"><BR>
</p> 


<br><br><input type="button" value="Порахувати" onclick="poschitat()">
            <input type="submit" value="Заказать" />
	            <input type="reset" value="Очистити" />

<p></p>
<div class="price">Ціна замовлення</div>
</form>
</body>
</html>
