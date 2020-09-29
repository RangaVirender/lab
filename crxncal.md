<style>
#calc{width:900px;height:650px;}
#btn{width:100%;height:40px;font-size:20px;}
</style>

<form Name="calc">
<table id="calc" border=0>
<tr>
<td colspan=1> Atomic no of projectile</td> <td colspan=1><input id="btn" name="disZproj" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<!--<td style="displayZproj:none"><input name="M" type="number"></td>-->
<td colspan=1></td>
<td colspan=1>Mass no of projectile</td> <td colspan=1><input id="btn" name="disAproj" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1></td>
</tr>
 
<tr>
<td colspan=1>Atomic no of target</td> <td colspan=1><input id="btn" name="disZtarget" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1></td>
<td colspan=1>Mass no of target</td><td colspan=1><input id="btn" name="disAtarget" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1></td>
</tr>

<tr>
<td colspan=1>Amount of charge incident on the target</td> <td colspan=1><input id="btn" name="disCharge" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>nano Coulomb</td>
<td colspan=1></td>
<td colspan=1>Charge state of projectile</td> <td colspan=1><input id="btn" name="disChargeState" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>In terms of charge on electon</td>
</tr>

<tr>
<td colspan=1>Areal density of target</td><td colspan=1><input id="btn" name="disAreal" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>g/cm3</td>
<td colspan=1></td>
<td colspan=1>Mass % of nuclei in the target</td><td colspan=1><input id="btn" name="disPercent" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>%</td>
</tr>

<tr>
<td colspan=1>Radius of the detector</td><td colspan=1><input id="btn" name="disRadius" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>cm</td>
<td colspan=1></td>
<td colspan=1>Distance of detector surface from target</td><td colspan=1><input id="btn" name="disDistance" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>cm</td>
</tr>

<tr>
<td colspan=1>Area under full energy peak</td><td colspan=1><input id="btn" name="disArea" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1></td><td colspan=1></td>
<td colspan=1>Full energy efficiency of detector</td><td colspan=1><input id="btn" name="disEff" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1></td>
</tr>

<tr>
<td colspan=2><input id="btn" type=button value="Calculate"
 OnClick="calc.disDiffCross.value=(
 calc.disArea.value*
 calc.disChargeState.value*1.6e-19*
 100.0*calc.disAtarget.value
 /
 (calc.disCharge.value*1.0e-9*
 calc.disAreal.value*calc.disPercent.value*
 6.022e23*calc.disEff.value*1.0e-27*
 2.0*3.14159*(1-calc.disDistance.value/(Math.sqrt(
                                                                                    Math.pow(calc.disRadius.value,2)+
                                                                                    Math.pow(calc.disDistance.value,2)
                                                                                   ))))).toPrecision(6),
calc.disTotalCross.value=(4.0*3.14159*calc.disDiffCross.value).toPrecision(6)"></td>
<td colspan=2><input id="btn" type=button value="Clear" 
OnClick="calc.disDiffCross.value=' ',
                calc.disTotalCross.value=' ',
                calc.disZproj.value=' ',
                calc.disAproj.value=' ',
                calc.disZtarget.value=' ',
                calc.disAtarget.value=' ',
                calc.disArea.value=' ',
                calc.disChargeState.value=' ',
                calc.disCharge.value=' ',
                calc.disAreal.value=' ',
                calc.disPercent.value=' ',
                calc.disEff.value=' ',
                calc.disDistance.value=' ',
                calc.disRadius.value=' ',
                calc.disDistance.value=' '"></td>
</tr>
<tr><td colspan=4>Differential Cross Section</td><td colspan=4>Total Cross Section</td>
</tr>

<tr>
<td colspan=2><input id="btn" name="disDiffCross" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=2>milli barn</td>
<td colspan=2><input id="btn" name="disTotalCross" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=2>milli barn</td>

</tr>
</table>
</form>
