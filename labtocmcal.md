## Lab energy to CoM energy convertor
<form Name="calc1">
<table id="calc">
<tr>
<td colspan=1>Lab Energy</td>
<td colspan=1><input id="btn" name="displayLabEnergy" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>MeV</td>
</tr>
<tr>
<td colspan=1>Mass no of projectile</td>
<td colspan=1><input id="btn" name="displayAproj" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
</tr>
<tr>
<td colspan=1>Mass no of target</td>
<td colspan=1><input id="btn" name="displayAtarget" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
</tr>
<tr>
<td colspan=1><input id="btn" type=button value="Calculate" OnClick="calc1.displayCMEnergy.value = (1.0*calc1.displayLabEnergy.value*calc1.displayAtarget.value/(1.0*calc1.displayAproj.value+1.0*calc1.displayAtarget.value)).toPrecision(6)"></td>
<td colspan=2><input id="btn" type=button value="Clear" OnClick="calc1.displayLabEnergy.value=' ',calc1.displayAproj.value=' ',calc1.displayAtarget.value=' ', calc1.displayCMEnergy.value=' '"></td>
</tr>
<tr>
<td colspan=1>CM Energy</td>
<td colspan=1><input id="btn" name="displayCMEnergy" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>MeV</td>
</tr>
</table>
</form>
## CoM energy to Lab energy convertor
<form Name="calc2">
<table id="calc">
<tr>
<td colspan=1>CoM Energy</td>
<td colspan=1><input id="btn" name="displayCMEnergy" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>MeV</td>
</tr>
<tr>
<td colspan=1>Mass no of projectile</td>
<td colspan=1><input id="btn" name="displayAproj" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
</tr>
<tr>
<td colspan=1>Mass no of target</td>
<td colspan=1><input id="btn" name="displayAtarget" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
</tr>
<tr>
<td colspan=1><input id="btn" type=button value="Calculate" OnClick="calc2.displayLabEnergy.value = (1.0*calc2.displayCMEnergy.value*(1.0*calc2.displayAproj.value+1.0*calc2.displayAtarget.value)/(1.0*calc2.displayAtarget.value)).toPrecision(6)"></td>
<td colspan=2><input id="btn" type=button value="Clear" OnClick="calc2.displayLabEnergy.value=' ',calc2.displayAproj.value=' ',calc2.displayAtarget.value=' ', calc2.displayCMEnergy.value=' '"></td>
</tr>
<tr>
<td colspan=1>Lab Energy</td>
<td colspan=1><input id="btn" name="displayLabEnergy" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
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
