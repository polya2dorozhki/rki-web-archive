# https://russianstepbystep.com/wp-content/uploads/2018/03/keyboard.html

- URL: https://russianstepbystep.com/wp-content/uploads/2018/03/keyboard.html
- Title: 
- Date: 
- Author: 

<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>Keyboard</title>
	<style>
		input.key
{
	padding-left:1ex; padding-right:1ex;
	padding-top: 0.5ex; padding-bottom: 0.5ex;
	width: 2.4em;
	height: 2.4em;
	margin-top: 2px;
	margin-bottom: 2px;
	margin-left: 0px;
	margin-right: 0px;
	vertical-align: text-center;
	align: center;
	font-weight: bold;
	font-size: 10pt;
	font-family: verdana;
}

input.bar
{
	padding-left:1ex; padding-right:1ex;
	padding-top: 0.5ex; padding-bottom: 0.5ex;
	height: 2.4em;
	margin-top: 1px;
	margin-bottom: 1px;
	vertical-align: text-center;
	align: center;
	font-weight: bold;
	font-size: 10pt;
	font-family: verdana;
}

input.space
{
	width: 10em;
}

p.keyboard
{
	margin-top: 0px;
	margin-bottom: 0px;
	padding-top: 0px;
	padding-bottom: 0px;
	
}
		</style>
	
	<script>
		var szyft = 0;
function shift() { if (szyft == 0) szyft = 1; else szyft = 0; }
function digit1() {updatepage("1", "!");}
function digit2(){updatepage("2","\"");};
function digit3(){updatepage("3","№");};
function digit4(){updatepage("4",";");};
function digit5(){updatepage("5","%");};
function digit6(){updatepage("6",":");};
function digit7(){updatepage("7","?");};
function digit8(){updatepage("8","*");};
function digit9(){updatepage("9","(");};
function digit0(){updatepage("0",")");};
function minus(){updatepage("-","_");};
function plus(){updatepage("=","+");};
function letter_jo(){ updatepage("ё", "Ё")}
function letter_shorti() { updatepage("й","Й"); }
function letter_tse() { updatepage("ц", "Ц"); }
function letter_u() { updatepage("у", "У"); }
function letter_ka() { updatepage("к","К"); }
function letter_ie() { updatepage("е","Е"); }
function letter_en() { updatepage("н","Н"); }
function letter_ghe() { updatepage("г","Г"); }
function letter_sha() { updatepage("ш","Ш"); }
function letter_shcha() { updatepage("щ","Щ"); }
function letter_ze() { updatepage("з","З"); }
function letter_ha() { updatepage("х","Х"); }
function letter_hard_sign() { updatepage("ъ","Ъ"); }
function letter_ef() { updatepage("ф","Ф"); }
function letter_yeru() { updatepage("ы","Ы"); }
function letter_ve() { updatepage("в","В"); }
function letter_a() { updatepage("а","А"); }
function letter_pe() { updatepage("п","П"); }
function letter_er() { updatepage("р","Р"); }
function letter_o() { updatepage("о","О"); }
function letter_el() { updatepage("л","Л"); }
function letter_de() { updatepage("д","Д"); }
function letter_zhe() { updatepage("ж","Ж"); }
function letter_e() { updatepage("э","Э"); }
function letter_ya() { updatepage("я","Я"); }
function letter_che() { updatepage("ч","Ч"); }
function letter_es() { updatepage("с","С"); }
function letter_em() { updatepage("м","М"); }
function letter_i() { updatepage("и","И"); }
function letter_te() { updatepage("т","Т"); }
function letter_soft_sign() { updatepage("ь","Ь"); }
function letter_be() { updatepage("б","Б"); }
function letter_yu() { updatepage("ю","Ю"); }
function kropka() { updatepage( "." , "," ); }
function slash() { updatepage("\\", "/"); }
function spacja() { updatepage(" "," "); }

function updatepage( bukwa1, bukwa2 )
{
  if (bukwa1 == ".")
  {
    if (szyft==0) 
		{ 
			insert(document.forms.textformularz.texterja, bukwa1);
			document.forms.textformularz.texterja.focus();
		};
    if (szyft==1) 
		{ 
			insert(document.forms.textformularz.texterja, bukwa2);
			document.forms.textformularz.texterja.focus();
		};
  }
  else
  {
    if (document.forms.capslockformularz.capslock.checked) { help=bukwa2; bukwa2=bukwa1; bukwa1=help; }
    if (szyft==1) { 
      //document.forms.textformularz.texterja.value += bukwa2; 
      insert(document.forms.textformularz.texterja, bukwa2);
      document.forms.textformularz.texterja.focus();
    }
    if (szyft==0) { 
      //document.forms.textformularz.texterja.value += bukwa1;
      insert(document.forms.textformularz.texterja, bukwa1);
      document.forms.textformularz.texterja.focus();
    }
  }
  szyft = 0;
}

// NEW FUNCTION
function insert(element,ins) {
    // gecko based
    if (element.setSelectionRange){
        var start = element.selectionStart;
        var end = element.selectionEnd;
        if (is_chrome) {
            start = selectionStart;
            end = selectionEnd;
        }
        element.value = element.value.substring(0,start) + ins + element.value.substring(end,element.value.length);

        start++;
        if (is_chrome) {
          selectionStart = start;
          selectionEnd = start;
        }

	element.selectionStart = start;
        element.selectionEnd = start;

    }
    // IE
    else if (document.selection && document.selection.createRange) {
        element.focus();
        var range = document.selection.createRange();
        range.text = ins;
	range.collapse(false);
        range.select();
    }
} 

function selectall()
{
 document.forms.textformularz.texterja.select();
}


var inputupper = new Array(
126,	//~
33,	//!
64,	//@
35,	//#
36,	//$
37,	//%
94,	//^
38,	//&
42,	//*
40,	//(
41,	//)
95,	//_
43,	//+
