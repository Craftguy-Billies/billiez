<textarea id="ta" style="width:90%;height:800px;"></textarea>

<input type="button" onclick="comma()" value="Commaification!">

<div id="display"></div>

<script>
function comma(){
var ta = document.getElementById("ta").value;
var r = [];
for (var i=0;i<ta.length;i++){
if(ta[i] == "\n"){
ta[i] = ", ";
}
r += ta[i];
}
var display = document.getElementById("display");
for(var i=0;i<r.length;i++){
display.innerHTML += r[i];
}
</script>
