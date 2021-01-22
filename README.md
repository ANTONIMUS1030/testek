<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title></title>
  <link rel="icon" type="image/png" href="http://pt.seaicons.com/wp-content/uploads/2016/03/Spy-icon.png" />
  <link href="https://fonts.googleapis.com/css?family=Roboto+Slab" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css" integrity="sha384-rHyoN1iRsVXV4nD0JutlnGaslCJuC7uwjduW9SVrLvRYooPp2bWYgmgJQIXwl/Sp" crossorigin="anonymous">
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
<style type="text/css">

  .form-control{
    width: 250px;
    text-align: center;
  }

  h4{
    font-family: 'Lobster', cursive;
    font-size: 30px;
  }
  body{
    margin-top: 25px;
  }
</style>
<center> <div style="width:103%;" class="card">
<div class="card-header"><h1></h1></h1><br>
                <center>
</script>
<form action="" name="form1" method="post">

    <input type="submit" class="btn btn-info" name="pesquisar" style="border-radius:0px;" value="Buscar Informações">
<br><br>

</center>

<?php
error_reporting(0);
set_time_limit(0);

//http://appservidor.suatela.com/ajax/appv/appv2_2_0_8.php?v=9.9.4&tipo=categoria&nome=episodios-serie-page&serie_id=43&serie_temporada=2&serie_audio=dublado&hwid=null

function getStr($string, $start, $end) {
    $str = explode($start, $string);
    $str = explode($end, $str[1]);
    return $str[0];
}
if(isset($_POST['pesquisar'])){
    
    $cpf = $_POST['nome'];

 $ch = curl_init();


//$ca = base64_encode($v);

curl_setopt($ch, CURLOPT_URL, 'Url');
curl_setopt($ch, CURLOPT_HEADER, 1);
curl_setopt($ch, CURLOPT_HTTPHEADER, array(
'HEADERS'
));
curl_setopt($ch, CURLOPT_USERAGENT, $_SERVER['HTTP_USER_AGENT']);
curl_setopt($ch, CURLOPT_RETURNTRANSFER, 1);
curl_setopt($ch, CURLOPT_FOLLOWLOCATION, 1);
curl_setopt($ch, CURLOPT_SSL_VERIFYPEER, 0);
curl_setopt($ch, CURLOPT_SSL_VERIFYHOST, 0);
curl_setopt($ch, CURLOPT_COOKIEFILE, getcwd().'/cookie.txt');
curl_setopt($ch, CURLOPT_COOKIEJAR, getcwd().'/COOKIE.TXT');
curl_setopt($ch, CURLOPT_POST, 1);
curl_setopt($ch, CURLOPT_POSTFIELDS, 'POST');  
$dados = curl_exec($ch);
 echo '<td><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTfGSv5sKqOiq9sJ_cl1A-8abpGwOzqkgFaDQ&usqp=CAU" "width="1000" height="105" /></td>';
 
echo '<br><br><td><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSm8aLA82fJF3w0v_-b6jk6bK_SeUvClnlCMw&usqp=CAU" "width="1000" height="105" /></td>';
        }

return;
    


?>
            <!-- #/ container -->
        </div>
        <!-- #/ content body -->
        <!-- footer -->
        <div class="footer">
            <div class="copyright">
                <p>Copyright &copy; <a href="#">SwagChks</a> 2020</p>
            </div>
        </div>

</html>
