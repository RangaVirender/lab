<form Name="calc">
<table id="calc">
<tr>
<td colspan=1> Atomic no of projectile</td> 
<td colspan=1><input id="btn" name="displayZproj" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<!--<td style="displayZproj:none"><input name="M" type="number"></td>-->
<td colspan=1>Mass no of projectile</td>
<td colspan=1><input id="btn" name="displayAproj" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
</tr>
<tr>
<td colspan=1>Atomic no of target</td>
<td colspan=1><input id="btn" name="displayZtarget" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>Mass no of target</td>
<td colspan=1><input id="btn" name="displayAtarget" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
</tr>
<tr>
<td colspan=2><input id="btn" type=button value="Calculate" OnClick="calc.displayCB.value=1.1998*calc.displayZproj.value*calc.displayZtarget.value/(Math.pow(calc.displayAproj.value,1/3)+Math.pow(calc.displayAtarget.value,1/3))"></td>
<td colspan=2><input id="btn" type=button value="Clear" OnClick="calc.displayCB.value=' ',calc.displayZproj.value=' ',calc.displayAproj.value=' ',calc.displayZtarget.value=' ',calc.displayAtarget.value=' '"></td>
</tr>
<tr>
<td colspan=2><input id="btn" name="displayCB" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=2>MeV</td>
</tr>
</table>
</form>

Please email me if you find any error.

---
![visitors](https://visitor-badge.glitch.me/badge?page_id=rangavirender.site.cbcal)

<p align="center">
<img src="logo_v1.png" width="30">
</p>
