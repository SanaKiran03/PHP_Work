<?php

$yr= 2004;
if (($yr%4==0)and ($yr%100!=0)){
echo ($yr . "is a laep year");
}
else if ($yr%400==0){
echo ($yr . "ia a laep year");
}
else {
	echo ($yr . "is not a laepyear");
	
}	

?>
