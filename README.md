IUG  
Web Programming 2 - SICT 2308  
ِِAssginment 4   
120171960
<!DOCTYPE html>
<html>
<head>
	<title></title>
</head>
<body>
	<?php
	$stdGrade = array("web1" => 90 , "DS" => 80 , "MC" => 75 , "P2" => 70);
	?>
	<table border="1">
		<tbody>
			<?php
			$total = 0;
			for (reset($stdGrade); $ky=key($stdGrade) ; next($stdGrade)) {
				$total += $stdGrade[$ky];
				?>
				<tr>
					<th><?php echo $ky?> </th>
					<td>
						<?php echo $stdGrade[$ky] ?>
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
