# PHPexercise

<!DOCTYPE html>
<html>
<head>
	<title>控制結構9-1-if敘述</title>
</head>
<body>
<?php
if(empty($_GET["username"])){
?>
<from action=<?php echo $_SERVER["PHP_SELF"]?> method="get">
我的名字叫作:<input type=text name=username> <br>
我是:<br>
<input type=radio name=sex value=1>男生<br>
<input type=radio name=sex value=2>女生<br>
<input type=submit value="送出">
<input type=reset value="重填">
</from>

<?php
/*><!--*/
//為何無法執行功能?
  }
  else
  {
    if($_GET["sex"]==1)
	echo $_GET["username"] ."先生您好";
    elseif ($_GET["set"]==2)
  	echo $_GET["username"] ."小姐您好";
    else
    {
      echo "尚未選擇您的性別<br>";
      echo "請重新選取<br>"; 
    }
   }
/*><!--*/
?>
</body>
</html>

//選項有出來，結果沒出來

