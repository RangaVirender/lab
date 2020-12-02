
<form Name="calc">
<table id="calc">
<tr>
<td colspan=1>Lab Energy</td>
<td colspan=1><input id="btn" name="displayLabEnergy" onkeypress="return event.charCode >= 48 && event.charCode <= 57" type="text"></td>
<td colspan=1>MeV</td>
</tr>
<tr>
<td colspan=1>Mass no of projectile</td>
<td colspan=1><input id="btn" name="displayAproj" onkeypress="return event.charCode >= 48 && event.charCode <= 57" type="text"></td>
</tr>
<tr>
<td colspan=1>Mass no of target</td>
<td colspan=1><input id="btn" name="displayAtarget" onkeypress="return event.charCode >= 48 && event.charCode <= 57" type="text"></td>
</tr>



<tr>
<td colspan=2><input id="btn" type=button value="Calculate" OnClick="calc.displayCMEnergy.value=calc.displayLabEnergy.value*calc.displayAtarget.value/(calc.displayAproj.value + calc.displayAtarget.value)"></td>
<td colspan=2><input id="btn" type=button value="Clear" OnClick="calc.displayCMEnergy.value=' ',calc.displayAproj.value=' ',calc.displayAtarget.value=' '"></td>
</tr>
<tr>
<td colspan=2><input id="btn" name="displayCMEnergy" onkeypress="return event.charCode >= 48 && event.charCode <= 57" type="text"></td>
<td colspan=1>MeV</td>
</tr>
</table>
</form>

Please email me if you find any error.

---
![visitors](https://visitor-badge.glitch.me/badge?page_id=rangavirender.site.labtocmcal)

<p align="center">
<img src="logo_v1.png" width="30">
</p>
