## Cross section calculator
<style>
#calc{width:980px;height:620px;}
</style>
<form Name="calc">
<table id="calc">
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
<td colspan=1>Charge state of projectile</td> <td colspan=1><input id="btn" name="disChargeState" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>units of e</td>
</tr>

<tr>
<td colspan=1>Areal density of target</td><td colspan=1><input id="btn" name="disAreal" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
 <td colspan=1>g cm<sup>-3</sup></td>
<td colspan=1>Mass % of nuclei in the target</td><td colspan=1><input id="btn" name="disPercent" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>%</td>
</tr>

<tr>
<td colspan=1>Radius of the detector</td><td colspan=1><input id="btn" name="disRadius" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>cm</td>
<td colspan=1>Distance of detector surface from target</td><td colspan=1><input id="btn" name="disDistance" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>cm</td>
</tr>

<tr>
<td colspan=1>Area under full energy peak</td><td colspan=1><input id="btn" name="disArea" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1></td>
<td colspan=1>Full energy efficiency of detector</td><td colspan=1><input id="btn" name="disEff" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1></td>
</tr>

<tr>
<td colspan=3><input id="btn" type=button value="Calculate"
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
<td colspan=3><input id="btn" type=button value="Clear" 
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
<tr><td colspan=3>Differential Cross Section</td><td colspan=4>Total Cross Section</td>
</tr>

<tr>
<td colspan=2><input id="btn" name="disDiffCross" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=1>milli barn</td>
<td colspan=2><input id="btn" name="disTotalCross" onkeypress="return event.charCode >= 42 && event.charCode <= 57" type="text"></td>
<td colspan=2>milli barn</td>

</tr>
</table>
</form>

<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>

$$
\dfrac{d\sigma(E,\theta)}{d\Omega}=\dfrac{Y}{N_pN_t\Omega\epsilon}
$$

Please email me if you find any error.

---
![visitors](https://visitor-badge.glitch.me/badge?page_id=rangavirender.site.crxncal)

<p align="center">
<img src="logo_v1.png" width="30">
</p>


