IUG  
Web Programming 2 - SICT 2308  
ِِAssginment 4   
id : 120171952
<!DOCTYPE html>
<html>
<head>
	<title></title>
</head>
<body>
	<?php
	 $Course = array("web2" => 85 , "DataBase" => 80 , "computerArt" => 77 , "Prog3" =>  98);
	<table border="1">
		<tbody>
			<?php
			$total = 0;
			for (reset($Course); $ky=key($Course) ; next($Course)) {
				$total += $Course[$ky];
				?>
				<tr>
					<th><?php echo $ky?> </th>
					<td>
						<?php echo $Course[$ky] ?>
					</td>
					</tr> <? } ?>
				</tbody>
				<tfoot>
					<tr>
						<th colspan="2">
							<? echo $total / 4; ?>
						</th>
					</tr>
				</tfoot>
			</table>
		</body>
		</html>
