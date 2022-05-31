Jmeter video播放压力测试


1.首先找到视频播放的接口 ( F12)



 这个接口中  Response Headers 中 Content-Length: 2639013 很重要，这个值返回的是文件的总大小，可以作为借口断言的依据



> 參考:

```
<?php
$file = $_GET['file'];
header ("Content-type: octet/stream");
header ("Content-disposition: attachment; filename=".$file.";");
header("Content-Length: ".filesize($file));
readfile($file);
exit;
?>

```
